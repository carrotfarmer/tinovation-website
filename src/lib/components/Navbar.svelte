<script>
  import { page } from "$app/stores";
</script>

<div class="fixed flex w-full flex-col items-center gap-4 py-4">
  <div>
    <nav
      class="text-semibold z-30 flex flex-row gap-4 rounded-3xl bg-retro-white px-4 py-1 font-header text-lg opacity-90 shadow-md shadow-transparent transition ease-in hover:-translate-y-0.5 hover:shadow-retro-white md:gap-8 md:px-10 md:py-1.5 md:text-2xl">
      {#if $page.url.pathname === "/"}
        <a href="/" class="text-amber-700 transition ease-in">home</a>
      {:else}
        <a href="/" class="transition ease-in hover:text-amber-700">home</a>
      {/if}

      {#if $page.url.pathname.includes("/resources")}
        <a href="/resources" class="text-pink-700 transition ease-in">resources</a>
      {:else}
        <a href="/resources" class="transition ease-in hover:text-pink-700">resources</a>
      {/if}

      {#if $page.url.pathname === "/showcase"}
        <a href="/showcase" class="text-blue-700 transition ease-in">showcase</a>
      {:else}
        <a href="/showcase" class="transition ease-in hover:text-blue-700">showcase</a>
      {/if}

      {#if $page.url.pathname === "/leaderboard"}
        <a href="/leaderboard" class="text-purple-700 transition ease-in">leaderboard</a>
      {:else}
        <a href="/leaderboard" class="transition ease-in hover:text-purple-700">leaderboard</a>
      {/if}
    </nav>
  </div>
  <div class="rounded-3xl bg-retro-white px-4 py-1 font-header text-2xl">
    Club Faire
    <a class="text-sky-700 underline" href="https://forms.gle/hvb6C1KAkU781qRX6"
      >interest forum →</a>
  </div>
</div>
