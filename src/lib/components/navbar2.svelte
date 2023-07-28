<script>
  import { navItems } from "$lib/config";
  import { page } from "$app/stores";
</script>

<div class=" flex list-none">
  {#each navItems as navItem}
    <li class:active_link={$page.url.pathname === `${navItem.path}`}>
      <a class="hover:text-primary-500 m-1" href={navItem.path}
        >{navItem.title}</a
      >
    </li>
  {/each}
</div>

<style>
  .active_link {
    color: rgba(var(--color-primary-500));
  }
</style>
