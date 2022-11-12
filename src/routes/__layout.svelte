<script lang="ts">
  import Header from '$lib/header/Header.svelte';
  import '../reset.css';
  import '../app.css';
</script>

<div>
  <main>
    <slot />
  </main>
</div>

<style>
  div {
    min-height: 100vh;
    display: grid;
    grid-auto-flow: row;
    grid-template-rows: auto 1fr;
    align-items: center;
    text-align: center;
  }
</style>
