<script lang="typescript">
    import AccordionItem from "./AccordionItem.svelte"

    export const projects = [
        {
            header: "DnD door",
            content: 'Dungeon door with magnetic base. Printed on Flashforge Adventurer 3 with FlashForge gray PLA. The door is from Fat Dragon Games starter set and the magnetic base is from Thingiverse.',
            img: "./assets/project_images/1_door.png",
            tag: "3d printing",
            alt: "A wooden door on a stone wall"
        },
        {
            header: "DnD floor",
            content: 'Dungeon floor with magnetic base. Printed on Flashforge Adventurer 3 with flashforge gray PLA. The floor tile is from Fat Dragon Games starter set and the magnetic base is from Thingiverse.',
            img: "./assets/project_images/2_floor.jpg",
            tag: "3d printing",
            alt: "Stone floor"
        },
        {
            header: "DnD wall",
            content: 'Single dungeon wall with magnetic base. Printed on Flashforge Adventurer 3 with flashforge gray PLA. The wall is from Fat Dragon Games starter set and the magnetic base is from Thingiverse.',
            img: "./assets/project_images/3_wall_single.jpg",
            tag: "3d printing",
            alt: "A stone wall"
        },
        {
            header: "DnD wall",
            content: 'Double dungeon wall with magnetic base. Printed on Flashforge Adventurer 3 with flashforge gray PLA. The wall is from Fat Dragon Games starter set and the magnetic base is from Thingiverse.',
            img: "./assets/project_images/4_wall_double.jpg",
            tag: "3d printing",
            alt: "Another stone wall"
        },
        {
            header: "Gift box",
            content: "Gift box printed on a Flashforge Adventure 3 with red and blue PLA from FlashForge. From the course run by Vladimir Mariano on Udemy.",
            img: "./assets/project_images/5_gift_box.png",
            tag: "3d printing",
            alt: "A gift box"
        },
        {
            header: "Ghost",
            content: "Ghost printed on a Flashforge Adventure 3 with transparent PLA from FlashForge. From the course run by Vladimir Mariano on YouTube.",
            img: "./assets/project_images/6_ghost.png",
            tag: "3d printing",
            alt: "A ghost"
        },
        {
            header: "Engine",
            content: "Engine benchmark printed on a Flashforge Adventure 3 with transparent PLA from FlashForge.",
            img: "./assets/project_images/7_engine.jpg",
            tag: "3d printing",
            alt: "An engine"
        },
        {
            header: "Batman spinner",
            content: "Batman spinner printed on a Flashforge Adventure 3 with black PLA from FlashForge.",
            img: "./assets/project_images/8_batman_spinner.jpg",
            tag: "3d printing",
            alt: "Batman spinner"
        },
        {
            header: "Batman spinner",
            content: "Batman spinner modelled in Fusion 360. From the course run by Vladimir Mariano on Udemy.",
            img: "./assets/project_images/Batman_spinner.png",
            tag: "3d modeling",
            alt: "Batman spinner 3d model"
        },
        {
            header: "Fidget spinner",
            content: "Geared fidget spinner modelled in Fusion 360. From the course run by Vladimir Mariano on Udemy.",
            img: "./assets/project_images/Geared_fidgetspinner.png",
            tag: "3d modeling",
            alt: "A geared fidget spinner"
        },
        {
            header: "Pumpkin bridge",
            content: "Pumpkin bridge modelled and rendered in Fusion 360. Designed by Tim Hellberg.",
            img: "./assets/project_images/Pumpkin_bridge.png",
            tag: "3d modeling",
            alt: "Pumpkin bridge"
        },
        {
            header: "Wonder woman tiara",
            content: "Wonder woman tiara modelled in Fusion 360. From the course run by Vladimir Mariano on Udemy.",
            img: "./assets/project_images/Wonderwoman_tiara.png",
            tag: "3d modeling",
            alt: "Wonder woman tiara"
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