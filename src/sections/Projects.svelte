<script>
    import Accordion from '../components/Accordion.svelte'
    import AccordionItem from '../components/AccordionItem.svelte'
</script>

<style lang="scss">
    @import '../../public/assets/variables';
    
    .projects-container {
        @include container-styles;

        h2 {
           @include h2-styles;
        }
    }
</style>

<div id="projects" class="projects">
    <div class="projects-container">
        <h2>Projects</h2>
        <Accordion/>
    </div>
</div>