<script>
  import { writable } from "svelte/store";

  const count = writable(0);

  function handleClick() {
    $count++;
  }

  $: doubled = $count * 2;
</script>

<div class="flex flex-col items-center gap-2">
  <p>
    Count: {$count}
  </p>
  <p>
    Doubled: {doubled}
  </p>
  <button
    class="rounded-xl bg-indigo-900 px-12 py-2 transition-colors hover:bg-indigo-700 active:bg-indigo-800"
    on:click={handleClick}
  >
    <slot />
  </button>
</div>
