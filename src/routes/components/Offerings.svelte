<script>
  import Arrow from '$lib/commonComponents/Arrow.svelte';
  const services = [
    'Advisory ',
    'Business Strategy',
    'Brand & Identity',
    'Change Management',
    'Coaching',
    'Customer & Marketing',
    'Digital Strategy & Transformation',
    'Enterprise Technology',
    'Human Capital',
    'Infrastructure & Information Security',
    'Leadership Development',
    'Management Consulting',
    'Operations',
    'Organizational Development',
    'People & Culture',
    'Program Development',
    'Scalability & Innovation',
    'Staff Augmentation',
    'Strategic Planning',
  ]
  const capabilities = [
    'AI / ML',
    'Analytics & Reporting',
    'App / Web Design & Development',
    'API Gateway',
    'Cloud Technology',
    'Communications & Media Systems ',
    'Data Fabric',
    'E-commerce & Marketplace',
    'Enterprise Automation',
    'Governance, Risk & Compliance',
    'Human-Centered UX Engineering',
    'ADA Usability Remediation & Compliance',
    'IoT & Digital Engineering',
    'Platform Engineering',
    'Quality Engineering',
    'Responsive Design & Optimization',
    'Software Development',
    'Unified Experience ',
  ]
  const industries = [
    'Aerospace & Defense',
    'Automotive',
    'Banking & Financial Services',
    'Capital Markets',
    'Chemicals',
    'Communications & Media',
    'Consumer Goods & Services',
    'Energy, Resources & Utilities',
    'Health',
    'High Tech, Software & Platform',
    'Industrial',
    'Insurance',
    'Life Sciences',
    'Logistics',
    'Natural Resources',
    'Public Service',
    'Retail',
    'Travel',
    'U.S. Federal Government',
  ]
</script>

<section class="offerings">
  <section class="services">
    <h3>Services <Arrow /></h3>
    <ul>
      {#each services as serv }
        <li>{serv}</li>
      {/each}
    </ul> 
  </section>
  <section class="capabilities">
    <h3>Capabilities <Arrow /></h3>
    <ul>
      {#each capabilities as cap }
        <li>{cap}</li>
      {/each}
    </ul> 
  </section>
  <section class="industries">
    <h3>Industries</h3>
    <ul>
      {#each industries as ind }
        <li>{ind}</li>
      {/each}
    </ul> 
  </section>
</section>

<style>
  .offerings {
    margin-top: 2rem;
    display: flex;
    flex-wrap: wrap;
    width: 100%;
  }
  .offerings section {
    background: white;
    flex-grow: 1;
    display: flex;
    flex-direction: column;
    flex-basis: 12.5rem;
  }
  ul {
    color: var(--primary);
    margin: 1rem 0.5rem 1rem 0;
    display: flex;
    flex-direction: column;
    flex-grow: 1;
  }
  li {
    margin: .2rem 0;
    flex-grow: 1;
  }
  h3 {
    padding: 1.5rem;
    font-size: 1.25rem;
    color: var(--primary);
    background: var(--grey1);
    margin: 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .capabilities h3 {
    background: var(--grey3);
  }
  .offerings .capabilities {
    background: var(--grey2);
  }
  @media all and (max-width: 800px) {
    .offerings section {
      flex-basis: 100%;
    }
  }
</style>