<script>
  import { navItems } from "$lib/config";
</script>

<div class="nav">
  <h1>Portfolio</h1>
  <div class="nav-list">
    {#each navItems as navItem}
      <li>
        <a href={navItem.path}> {navItem.title}</a>
      </li>
    {/each}
  </div>
</div>

<style>
  * {
    margin: 10px;
  }

  .nav {
    display: flex;
    justify-content: space-between;
  }
  .nav-list {
    list-style-type: none;
    display: flex;
    text-decoration: none;
  }
</style>
