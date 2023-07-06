<script>
  import "@skeletonlabs/skeleton/themes/theme-crimson.css";
  import "@skeletonlabs/skeleton/styles/skeleton.css";
  import "../app.postcss";
  import { AppShell } from "@skeletonlabs/skeleton";
  import { AppBar } from "@skeletonlabs/skeleton";
  import Navbar from "$lib/components/navbar.svelte";
</script>

<AppShell>
  <svelte:fragment slot="pageHeader">
    <Navbar logo="pofo.dev" />
  </svelte:fragment>
  <slot />
</AppShell>

<style>
</style>
