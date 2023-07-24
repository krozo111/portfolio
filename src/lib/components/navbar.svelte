<script>
  import { navItems } from "$lib/config";
  import Icon from "@iconify/svelte";
  import { page } from "$app/stores";
</script>

<header
  class="bg-surface-200 dark:bg-surface-700 lg:w-[560px] h-[144px] lg:block p-[30px] ml-auto mb-10 rounded-[16px]"
>
  <nav class=" lg:block">
    <ul class="flex justify-between font-semibold">
      {#each navItems as navItem}
        <li
          class="rounded-lg bg-surface-50 dark:bg-surface-900"
          class:active_link={$page.url.pathname === `${navItem.path}`}
        >
          <a
            class="flex cursor-pointer flex-col items-center justify-center rounded-lg w-20 h-20"
            href={navItem.path}
          >
            <span class="text-xl mb-1">
              <Icon icon={navItem.icon} width="24" />
            </span>
            {navItem.title}
          </a>
        </li>
      {/each}
    </ul>
  </nav>
</header>

<style>
  .active_link {
    background: linear-gradient(
      to top,
      rgb(236, 72, 153),
      rgb(239, 68, 68),
      rgb(234, 179, 8)
    );
  }
</style>
