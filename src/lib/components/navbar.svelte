<script>
  import { navItems } from "$lib/config";
</script>

<nav class="nav">
  <h1>Jorge Corzo<span class="color">[<span>-</span>]</span></h1>
  <div class="nav__div">
    {#each navItems as navItem}
      <li>
        <a href={navItem.path}> {navItem.title}</a>
      </li>
    {/each}
  </div>
</nav>

<style>
  * {
    margin: 10px;
    padding: 10px;
    text-decoration: none;
  }

  .color {
    color: var(--colorSecundary);
  }
  .nav {
    display: flex;
    justify-content: space-between;
    margin-top: 20px;
    align-items: center;
  
  }
  .nav__div {
    display: flex;
    list-style-type: none;
 
  }

  .nav__div :hover {
    color: var(--colorSecundary);
  }

</style>
