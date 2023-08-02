<script>
  import Customer from "$lib/components/customer.svelte";
  import Skills from "$lib/components/skills.svelte";
  import About from "$lib/components/about.svelte";
  
  import SideNav from "$lib/components/sideNav.svelte";
</script>

<div class="lg:hidden">
<SideNav />
</div>
<About />
<Skills />
<Customer />


