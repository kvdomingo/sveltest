<script>
  import CounterButton from "$lib/CounterButton.svelte";
</script>

<div
  class="flex h-screen w-full flex-col items-center justify-center gap-4 bg-gradient-to-b from-orange-900 to-orange-950"
>
  <h1>Welcome to SvelteKit!</h1>
  <p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
  <CounterButton>count!</CounterButton>
</div>

<style lang="postcss">
  :global(body) {
    background-color: theme(colors.sky.950);
    color: white;
    font-size: 14pt;
  }
  :global(h1) {
    font-size: theme(fontSize.4xl);
  }
  :global(h2) {
    font-size: theme(fontSize.3xl);
  }
  :global(h3) {
    font-size: theme(fontSize.2xl);
  }
  :global(h4) {
    font-size: theme(fontSize.xl);
  }
  :global(h5) {
    font-size: theme(fontSize.lg);
  }
  :global(a) {
    color: theme(colors.sky.300);
  }
</style>
