---
section: configure
title: Workspace Classes
---

<script context="module">
  export const prerender = true;
</script>

# {title}

> {title} are currently in [early access](/docs/references/gitpod-releases) · [Send feedback](https://github.com/gitpod-io/gitpod/issues/12473).

Workspace classes allow you to select the resources that are assigned to your workspace.

You can configure the workspace class that should be used for your workspaces in your personal preferences.

![Select Workspace Class](../../../static/images/docs/select-workspace-class.png)

Once you have selected the workspace class every new workspace will use the updated workspace class.

## Good to know

- Your existing workspaces will continue to use the workspace class that they have been created with.
- Prebuilds will use the workspace class preference of the installation owner.
- If a prebuild exists and your configured workspace class is not sufficient to use the prebuild, the workspace
  created from that prebuild will use the workspace class of the prebuild instead of the configured one.
