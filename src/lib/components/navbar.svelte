<script>
  // @ts-nocheck

  import { navItems } from "$lib/config";
  import { page } from "$app/stores";
  export let logo;
</script>

<nav class="m-3 p-1 flex justify-between mt-5 items-center">
  <h1>{logo}</h1>
  <div class="flex list-none ">
    {#each navItems as navItem}
      <li class:active_link={$page.url.pathname === `${navItem.path}`}>
        <a class="hover:text-red-600 p-4" href={navItem.path}>{navItem.title}</a>
      </li>
    {/each}
  </div>
</nav>

<style>
  /* * {
    margin: 10px;
    padding: 5px;
    text-decoration: none;
  }

  .nav {
    display: flex;
    justify-content: space-between;
    margin-top: 20px;
    align-items: center;
  }
  a:visited {
    color: inherit;
  }
  .nav__div {
    display: flex;
    list-style-type: none;
  }

  .nav__div :hover {
    color: var(--colorSecundary);
  }

  .active_link {
    color: var(--colorSecundary);
  } */
</style>
