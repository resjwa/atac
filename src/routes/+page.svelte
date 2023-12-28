<script lang="ts">
  import Hero from './components/Hero.svelte';
  import '../global.css';
  import Logo from '$lib/commonComponents/Logo.svelte';
</script>

<svelte:head>
  <title>MilCloud</title>
</svelte:head>

<div class="layout">
  <header>
    <Logo />
  </header>
  <Hero />
</div>

<style>
  .layout {
    position: relative;
    max-width: 1240px;
    width: 100%;
    display: block;
    margin: 0 auto;
  }
  header {
    display: flex;
    align-items: center;
    justify-content: flex-start;
  }
</style>
