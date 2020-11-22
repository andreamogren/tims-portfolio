<script>
    import * as animateScroll from "svelte-scrollto";

    const menuItems = [
        'Projects', 'About', 'Contact'
    ]
</script>

<style lang="scss">
    @import '../../public/assets/variables';

    header {
        background-color: #f8f9fa;
        position: fixed;
        width: 100%;
        z-index: 10;
    }

    .header-container {
        max-width: $container-width;
        margin: 0 auto;
        padding: calc(#{$base-padding} * 2) 0;
        display: flex;
        justify-content: space-between;    

        a {
            text-decoration: none;
            color: $primary-color;
            font-size: 18px; 
            font-weight: 700;
            margin-right: calc(#{$base-padding} * 2);
            margin-left: $base-padding;   

            @media(min-width: $desktop-min-width) {
                margin-left: 0;
            }
        }

        a:hover {
            color: $secondary-color;
        }
    }
</style>

<header>
    <div class="header-container">
        <a on:click={() => animateScroll.scrollTo({element: "#start"})} href="#start" class="name">Tim Hellberg</a>
        <nav class="menu">
                {#each menuItems as item}
                    <a on:click={() => animateScroll.scrollTo({element: `#${item.toLowerCase()}`})} href="#{item}">
                        {item}
                    </a>
                {/each}
        </nav>
    </div>
</header>