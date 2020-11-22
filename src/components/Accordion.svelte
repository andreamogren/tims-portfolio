<script lang="typescript">
    import AccordionItem from "./AccordionItem.svelte"

    export const projects = [
        {
            header: "aweee",
            content: "I am a little cat mjuuu I am a little cat mjuuu I am a little cat mjuuuI am a little cat mjuuu v I am a little cat mjuuuI am a little cat mjuuu v I am a little cat mjuuuI am a little cat mjuuuI am a little cat mjuuuv I am a little cat mjuuuI am a little cat mjuuu I am a little cat mjuuu ",
            img: "https://thefloridavillager.com/wp-content/uploads/2020/06/cat-mask-750x460.jpg",
            tag: "3d printing",
            alt: "test"
        },
        {
            header: "aweee",
            content: "I am a little cat mjuuu",
            img: "https://thefloridavillager.com/wp-content/uploads/2020/06/cat-mask-750x460.jpg",
            tag: "3d modeling",
            alt: "test"
        },
        {
            header: "aweee",
            content: "I am a little cat mjuuu",
            img: "https://thefloridavillager.com/wp-content/uploads/2020/06/cat-mask-750x460.jpg",
            tag: "3d printing",
            alt: "test"
        },
        {
            header: "aweee",
            content: "I am a little cat mjuuu",
            img: "https://thefloridavillager.com/wp-content/uploads/2020/06/cat-mask-750x460.jpg",
            tag: "3d modeling",
            alt: "test"
        },
    ]
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