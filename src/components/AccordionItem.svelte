<script lang="typescript">
    export let content: string
    export let header: string
    export let img: string
    export let alt: string
    export let tag: string
    export let thingiverseLink: string
    export let fatDragonLink: string

    let isOpen = false

    const toggleAccordion = () => {
        isOpen = !isOpen
    }
</script>

<style lang="scss">
@import '../../public/assets/variables';

.accordion-item {
    margin-bottom: $base-padding;
    > img {
        width: 358px;
        height: 270px;
        max-height: 100%;
        max-width: calc(100% - 2px);
        border: 1px solid lightgray;
    }

    @media (min-width: $tablet-max-width) {
        margin-right: $base-padding;
        width: calc(50% - #{$base-padding});
    }

    @media (min-width: $desktop-min-width) {
        width: calc(33% - #{$base-padding});
    }

    @media (max-width: $mobile-max-width) {
        max-width: 100%;
    }
}

.accordion-item-header {
    display: flex;
    align-items: center;
    flex-wrap: nowrap;
    justify-content: space-between;
    padding: 0 $base-padding;
    border: solid $primary-color 1px;
    border-top: 0;
    border-radius: 4px;
    border-top-left-radius: 0;
    border-top-right-radius: 0;
    margin-top: -5px;

    & > p {
        font-weight: 600;
    }

    .icon-container {
        display: flex;
        align-items: center;

        .arrow-icon {
            width: 20px;
            height: 20px;
            margin-left: $base-padding;
            transition: 0.3s;
        }

        .tag {
            font-size: 13px;
            padding: calc(#{$base-padding} / 2 ) $base-padding;
            border-radius: 8px;

            &.printing {
                background-color: $primary-color;
            }

            &.modeling {
                background-color: $secondary-color;
            }
        }
    }
}

.accordion-item-body {
    padding: 0 $base-padding $base-padding;
    border: solid $primary-color 1px;
    border-radius: 4px;
    border-top-left-radius: 0;
    border-top-right-radius: 0;

    a {
        display: block;
        margin-bottom: calc(#{$base-padding} / 2);
        color: $secondary-color;
        font-weight: 700;
        text-decoration: none; 
    }
}

.accordion-item.selected {
    .accordion-item-header {
        border-bottom: transparent 1px solid;
        border-radius: 0;
    }

    .arrow-icon {
        transform: rotate(180deg);
    }

    .accordion-item-body {
        border-top: transparent 1px solid;
    }
}
</style>

<div class={isOpen ? "accordion-item selected": "accordion-item"}>
    <img src={img} alt={alt}/>
    <div class="accordion-item-header" on:click={toggleAccordion}>
        <p>{header}</p>
        <div class="icon-container">
            <p class="tag {tag}">{tag}</p>
            <img class="arrow-icon" src="./assets/chevron-arrow-down.svg" alt="">
        </div>
    </div>
    {#if isOpen}
        <div class="accordion-item-body">
            <p>{content}</p>
            {#if thingiverseLink}
                <a href={thingiverseLink} target="_blank" rel="noopener noreferrer">Link to Thingiverse</a>
            {/if}
            {#if fatDragonLink}
                <a href={fatDragonLink} target="_blank" rel="noopener noreferrer">Link to Fat Dragon Games</a>
            {/if}
        </div>
    {/if}
</div>