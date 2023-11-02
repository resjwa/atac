<script lang="ts">
  import { browser } from '$app/environment';
  import Hero from './components/Hero.svelte';
  import '../global.css';
  import Offerings from './components/Offerings.svelte';
  import Logo from '$lib/commonComponents/Logo.svelte';
  let AAAdmin: string | null = '';
  if (browser) {
    AAAdmin = localStorage.getItem('AAAdmin');
  }
</script>
<div class="layout">
  <header>
    <Logo />
  </header>
  <main>
    <Hero />
    {#if AAAdmin === 'true'}
      <Offerings />
    {/if}
  </main>
</div>
<style>
  .layout {
    max-width: 1240px;
    width: 100%;
    display: block;
    margin: 0 auto;
  }
</style>
