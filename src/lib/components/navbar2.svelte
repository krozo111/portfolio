<script>
  // @ts-nocheck

  import { navItems } from "$lib/config";
  import { page } from "$app/stores";
  import { LightSwitch } from '@skeletonlabs/skeleton';
  export let logo;
</script>

<nav class="flex items-center justify-between flex-wrap p-10">
  <h1 class="h1 my-4"><span class="text-primary-500">&lt</span> {logo} <span class="text-primary-500">&gt</span></h1>
  
  <div class="hidden my-4 md:flex list-none items-center flex-shrink-0">
    {#each navItems as navItem}
      <li class:active_link={$page.url.pathname === `${navItem.path}`}>
        <a class="hover:text-primary-500 m-10 " href={navItem.path}>{navItem.title}</a>
      </li>
    {/each}
    <LightSwitch />
  </div>
</nav>

<style>
 .active_link {
  color: rgba(var(--color-primary-500));
 }
</style>
