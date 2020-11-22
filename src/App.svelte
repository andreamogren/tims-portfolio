<script>
  import Menu from './components/Menu.svelte'
  import Hero from './sections/Hero.svelte'
  import Projects from './sections/Projects.svelte'
  import About from './sections/About.svelte'
  import Contact from './sections/Contact.svelte'
  import Footer from './components/Footer.svelte'
</script>

<style lang="scss">
  @import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;600;700&display=swap');
  @import '../public/assets/variables';
  :global(body) {
    margin: 0;
    background-color: #ffffff;
    font-family: 'Open Sans', sans-serif;
  }
</style>

<Menu/>
<Hero/>
<Projects/>
<About/>
<Contact/>
<Footer/>
