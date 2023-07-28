<script>
  import Navbar2 from "./navbar2.svelte";
  import { LightSwitch } from "@skeletonlabs/skeleton";
  let visible = true;
</script>

<div
  class="bg-surface-200 dark:bg-surface-900 w-full
        flex justify-between px-5 fixed top-0 
        items-center">

  <LightSwitch />
  {#if !visible}
    <Navbar2 />
  {/if}
  <button
    type="button"
    class="btn-icon variant-filled-surface z-10"
    on:click={() => (visible = !visible)}
    ><iconify-icon icon="mdi:menu" />
  </button>
</div>
