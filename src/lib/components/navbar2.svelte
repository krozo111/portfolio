<script>
  import { navItems } from "$lib/config";
  import { page } from "$app/stores";
  import { LightSwitch } from '@skeletonlabs/skeleton';
</script>


  <div class=" z-10 flex flex-wrap items-center justify-around pt-6 list-none">
    {#each navItems as navItem}
      <li class:active_link={$page.url.pathname === `${navItem.path}`}>
        <a class="hover:text-primary-500 m-10 " href={navItem.path}>{navItem.title}</a>
     <br>
      </li>
    {/each} 
    <LightSwitch />
   
     
    
  </div>

<style>
 .active_link {
  color: rgba(var(--color-primary-500));
 }
</style>
