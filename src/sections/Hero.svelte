<style lang="scss">
    @import '../../public/assets/variables';

    .hero-container {
        background-image: url("./assets/boat.jpg");
        background-repeat: no-repeat;
        background-position: center center;
        background-size: cover;
    }

    .hero-content {
        @include container-styles;
        min-height: 500px;
        color: #fff;
        display: flex; 
        align-items: center;

        h1 {
            font-size: $h1-size;
        }
    }
</style>

<div id="start" class="hero-container">
    <div class="hero-content">
        <div>
            <h1>Hello I'm Tim!</h1>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
        </div>
    </div>
</div>