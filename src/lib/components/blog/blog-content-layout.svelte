<script lang="ts">
  import RecentArticlesPreview from "./recent-articles-preview.svelte";
  import PostContentLayout from "../post-content-layout.svelte";
  import FeedbackWidget from "../docs/feedback-widget.svelte";
  import DigestHeader from "./digest-header.svelte";
  const { type } = $$restProps;
</script>

<PostContentLayout
  imagesDirectoryName="blog"
  baseUrl="https://www.gitpod.io/blog/"
  {...$$restProps}
>
  <slot />
  {#if type === "digest"}
    <DigestHeader />
  {/if}
</PostContentLayout>

{#if type === "digest"}
  <FeedbackWidget class="mt-large mb-huge" type="digests" />
{/if}
<RecentArticlesPreview />
