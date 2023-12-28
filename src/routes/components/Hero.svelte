<section class="hero-content">
  <p class="tagline">Tagline</p>
  <h2>Military readiness requires mission-minded solutions</h2>
  <div class="copy">
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Saepe aliquam
      alias id, temporibus nobis fugit nemo doloremque ipsa consectetur nisi rem
      ullam error eos consequuntur fugiat. Ea ut cum laborum? Lorem ipsum dolor
      sit amet consectetur adipisicing elit. Saepe aliquam alias id, temporibus
    </p>
    <p class="cta">
      <a href="mailto:contact@milcloud.com?subject=Website Inquiry">email us</a>
      at contact@milcloud.com
    </p>
  </div>
</section>

<style lang="scss">
  .cta {
    border: 2px solid var(--lightText);
    border-radius: 4px;
    padding: 1rem 2rem;
    width: auto;
    display: inline-block;
  }
  p {
    max-width: 31rem;
  }
  .copy {
    border-left: 1px solid var(--lightText);
    padding-left: 2.5rem;
  }
  h2 {
    max-width: 43rem;
  }
  .tagline {
    margin: 0;
    font-size: 1.0625rem;
    font-style: normal;
    font-weight: 300;
    text-transform: uppercase;
  }
  .hero-content {
    position: relative;
    padding: 5rem;
  }

  @media screen and (max-width: 768px) {
    .hero-content {
      position: relative;
      padding: 3rem;
    }
  }
  @media screen and (max-width: 480px) {
    h2 {
      font-size: 2.25rem;
      line-height: 2.8125rem;
      max-width: 100%;
    }
    .hero-content {
      position: relative;
      padding: 2rem 1rem;
    }
    .copy {
      padding-left: 1rem;
    }
  }
</style>
