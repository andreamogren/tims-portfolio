<style lang="scss">
    @import '../../public/assets/variables';

    .about {
        background-color: #e6f3f1;
    }

    .about-container {
        @include container-styles;
    }

    h2 {
        @include h2-styles;
    }

    .text-content-container {
        display: flex;
        align-items: center;
        position: relative;
        flex-wrap: wrap;
        justify-content: center;

        p {
            max-width: 690px;
        }

        img {
            border: 1px solid black;
            width: 400px;
            max-width: 100%;
        }

        @media(min-width: $desktop-min-width) {
            justify-content: flex-start;

            img {
                position: absolute;
                right: 0;
            }   
        }
    }
</style>

<div id="about" class="about">
    <div class="about-container">
        <h2>About</h2>
        <div class="text-content-container">
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
            <img src="https://i.pinimg.com/originals/3a/fb/f8/3afbf8c348fb977671a5e41d83e39bee.jpg" alt="An image of Tim"/>
        </div>
    </div>
</div>