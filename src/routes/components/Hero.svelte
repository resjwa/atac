<script>
  import Sphere from './SphereAnimation.svelte';
</script>
<section class="hero-content">
  <p class="tagline">WE ARE A GLOBAL PROFESSIONAL SERVICES COMPANY</p>
  <h2>The promise of human empowerment in the age of AI</h2>
  <div class="copy">
    <p>AtomicAcumen delivers a comprehensive array of services, capabilities, and solutions that span multiple industries, including deep expertise in strategy, operations, and information technology. We help businesses, government entities, and military organizations maximize operational impact, create sustainable value, and improve human lives by transforming complexity into competitive advantage. Headquartered in Nashville, Tennessee, AtomicAcumen maintains additional offices in Austin, Texas, and the Washington metropolitan area.</p>
    <p class="cta"><a href="mailto:hello@atomicacumen.com?subject=Website Inquiry">email us</a> at hello@atomicacumen.com</p>
  </div>
  <Sphere />
</section>
<style>
  .tagline {
    margin: 0;
  }
  .tagline, .cta {
    font-size: 1.0625rem;
    font-style: normal;
    font-weight: 300;
    text-transform: uppercase;
  }
  .copy {
    border-left: 1px solid #6B6B6B;
    padding-left: 2.5rem;
  }
  .hero-content {
    position: relative;
    padding-top: 5rem;
  }
  .cta {
    border: 2px solid #ff7535;
    border-radius: 4px;
    padding: 1rem 2rem;
    width: auto;
    display: inline-block;
  }
  @media screen and (max-width: 1000px) {
    .tagline {
      font-size: 1rem;
      margin-bottom: 1rem;
    }
  }
  @media screen and (max-width: 480px) {
    h2 {
      font-size: 2.25rem;
      line-height: 2.8125rem;
      max-width: 100%;
    }
    .copy {
      padding-left: 0;
      border-left: 0;
    }
    .copy p:first-child {
      border-left: 1px solid #6b6b6b;
      padding-left: 1.313rem;
    }
    .cta {
      font-size: 0.9rem;
    }
    .hero-content {
      position: relative;
      padding-top: 1rem;
    }
  }
</style>