<script>
  import Arrow from '$lib/commonComponents/Arrow.svelte';
  const services = [
    'Brand, Identity & Marketing',
    'Digital Strategy & Transformation',
    'Engagement & Readiness',
    'Infrastructure & Information Security',
    'Organizational Development',
    'People, Culture & Retention',
    'Scalability & Innovation',
  ];
  const capabilities = [
    'AI / ML / Data tools',
    'Automation, Analytics & Reporting',
    'Governance, Risk & Compliance',
    'Human-Centered UX Engineering',
    'ADA Remediation & Compliance',
    'Software Development',
  ];
</script>

<section class="offerings">
  <section class="mainCopy">
    <h3>
      The intelligent platform for end-to-end readiness <span class="arrow"
        ><Arrow /></span
      >
    </h3>
    <p>
      MilCloud – a proud and exclusive U.S. strategic partner in military cloud
      solutions – enables comprehensive digital transformation for military
      readiness. In the present dynamic landscape, legacy 20th-century IT
      systems render organizations vulnerable to sudden disruptions and cyber
      attacks. Recent geopolitical events highlight the need for adaptable,
      durable, and resilient digital infrastructure.
    </p>

    <p>
      As U.S. leaders navigate global challenges, readiness becomes paramount.
      Current affairs demonstrate that major threats transcend borders and
      necessitate decisive action. Pandemics, biological risks, the climate
      crisis, cyber threats, economic disruptions, humanitarian crises,
      extremism, terrorism, and the proliferation of weapons pose profound and
      existential dangers.
    </p>

    <p>
      To safeguard U.S. national security and deter war amid today's complex
      landscape, military organizations must digitally transform. The essence
      lies in delivering person-centered, mission-minded experiences in a modern
      context. By optimizing critical processes, MilCloud guarantees an
      uninterrupted flow of work across people, data, and systems. Prepare for
      today and tomorrow with MilCloud – where agility seamlessly intertwines
      with innovation in military cloud solutions.
    </p>
  </section>
  <aside>
    <section class="services">
      <h3>Services</h3>
      <ul>
        {#each services as serv}
          <li>{serv}</li>
        {/each}
      </ul>
    </section>
    <section class="capabilities">
      <h3>Capabilities</h3>
      <ul>
        {#each capabilities as cap}
          <li>{cap}</li>
        {/each}
      </ul>
    </section>
  </aside>
</section>

<style lang="scss">
  .offerings {
    display: flex;
    flex-wrap: wrap;
    width: 100%;
  }
  .mainCopy {
    background: white;
    display: flex;
    flex-direction: column;
    flex-basis: 67%;
    h3 {
      padding-left: 5rem;
    }
    p {
      padding-left: 5rem;
      padding-right: 5rem;
      max-width: 45rem;
    }
  }
  .arrow {
    margin-left: 0.5rem;
  }
  aside {
    display: flex;
    flex-direction: column;
    flex-basis: 33%;
    background: var(--grey2);
    section {
      flex-basis: 50%;
    }
    h3,
    ul {
      padding-left: 2rem;
    }
    li {
      margin-left: 1rem;
    }
  }
  ul {
    color: var(--primary);
    margin: 1rem 0.5rem 2rem 0;
    display: flex;
    flex-direction: column;
    flex-grow: 1;
  }
  li {
    margin: 0.2rem 0;
  }
  h3 {
    padding: 1.5rem;
    font-size: 1.25rem;
    color: var(--primary);
    background: var(--grey1);
    margin: 0;
    display: flex;
    justify-content: flex-start;
    align-items: center;
  }
  .capabilities h3,
  .services h3 {
    background: var(--grey3);
  }
  .capabilities,
  .services {
    background: var(--grey2);
  }
  @media all and (max-width: 900px) {
    aside,
    .mainCopy {
      flex-basis: 100%;
    }
    .services {
      h3,
      ul {
        padding-left: 5rem;
      }
    }
  }
  aside {
    flex-direction: row;
    flex-wrap: wrap;
    section {
      flex-grow: 1;
      flex-basis: 18rem;
    }
  }
  @media all and (max-width: 768px) {
    .offerings .mainCopy {
      h3 {
        padding-left: 3rem;
      }
      p {
        padding-left: 3rem;
        padding-right: 3rem;
      }
    }
    .offerings aside {
      h3,
      ul {
        padding-left: 3rem;
      }
    }
  }
</style>
