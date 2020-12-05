<script lang="typescript">
    import AccordionItem from "./AccordionItem.svelte"
    import projects from "../projects"


</script>

<style lang="scss">
    @import '../../public/assets/variables';
    
    .accordion {
        display: flex;
        flex-wrap: wrap;
        padding: calc(#{$base-padding} * 2) 0;
    }
</style>



<div class="accordion">
    {#each projects as project}
        <AccordionItem {...project}/>
    {/each}
</div>