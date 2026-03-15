<script lang="ts">
  import { onMount } from 'svelte';

  let dark = false;

  onMount(() => {
    const saved = localStorage.getItem('theme');
    dark = saved ? saved === 'dark' : window.matchMedia('(prefers-color-scheme: dark)').matches;
    applyTheme();
  });

  function applyTheme() {
    if (dark) {
      document.documentElement.setAttribute('data-theme', 'dark');
      localStorage.setItem('theme', 'dark');
      return;
    }

    document.documentElement.removeAttribute('data-theme');
    localStorage.setItem('theme', 'light');
  }

  function toggleTheme() {
    dark = !dark;
    applyTheme();
  }
</script>

<button class="theme-toggle" type="button" on:click={toggleTheme}>
  {dark ? 'dark' : 'light'}
</button>

<style>
  .theme-toggle {
    position: fixed;
    top: 1rem;
    right: 1rem;
    border: 1px solid var(--card-border);
    background: var(--card-bg);
    color: var(--text);
    font-family: 'DM Mono', monospace;
    font-size: 0.82rem;
    text-transform: lowercase;
    border-radius: 999px;
    padding: 0.4rem 0.8rem;
    cursor: pointer;
    backdrop-filter: blur(8px);
    z-index: 10;
  }
</style>
