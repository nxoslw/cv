<script>
  import Section from '../components/Section.svelte';
  import Intro from '../components/Intro.svelte';
  /*import ForkMe from '../components/ForkMe.svelte';*/

  import Hello from '../content/01-hello.md';
  import Experience from '../content/02-experience.md';
  import Skills from '../content/03-skills.md';
  import Education from '../content/04-education.md';
  import Hobby from '../content/05-hobby.md';
  import Footer from '../content/06-footer.md';

  const sections = [
    { id: 'hello', component: Hello },
    { id: 'experience', component: Experience },
    { id: 'skills', component: Skills },
    { id: 'education', component: Education },
    { id: 'hobby', component: Hobby },
  ];
</script>

<svelte:head>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link rel="preconnect" href="https://nxo.codes" crossorigin>
  <link rel="preconnect" href="https://www.nxo.codes" crossorigin>
  <link
    href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@200;400;600&display=swap"
    rel="stylesheet"
  />
</svelte:head>

<Intro />

<main>
  {#each sections as section}
    <Section id={section.id}>
      <svelte:component this={section.component} />
    </Section>
  {/each}

  <picture>
    <source srcset="images/nxo-sm.webp" type="image/webp" media="(max-width: 480px)">
    <source srcset="images/nxo-md.webp" type="image/webp" media="(max-width: 800px)">
    <source srcset="images/nxo.webp" type="image/webp" media="(min-width: 801px)">
    <source srcset="images/nxo.jpg" type="image/jpeg" media="(min-width: 801px)">
    <img src="images/nxo.jpg" alt="nxo" id="me" loading="lazy">
  </picture>
</main>

<footer id="footer">
  <Footer />
</footer>

<!--<ForkMe />-->
<!-- Google Tag Manager (noscript) -->
<noscript><iframe src="https://www.googletagmanager.com/ns.html?id=GTM-P9DWD6QH"
height="0" width="0" style="display:none;visibility:hidden"></iframe></noscript>
<!-- End Google Tag Manager (noscript) -->

<style lang="scss" global>
  @import '../styles/global';

  #me {
    width: 100vw;
    object-fit: cover;
  }

  #footer {
    background-color: darken($background-color, 2%);
    font-size: 0.875em;
    padding-block: 3em;
    text-align: center;
  }
</style>
