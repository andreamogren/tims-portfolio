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
            <p>Hello and welcome to my portfolio! My name is Tim and I'm currently a student at Xenters 3D-Technician program. I aspire to become someone with have broad understanding of the field that I'm working in. At my workplace my goal will be that machines are never broken and keept in tiptop condition. I'm a curious nerd that loves games and even more to cook. Mexican is my cuisine of choice.</p>
            <img src="./assets/tim_hellberg.jpg" alt="An image of Tim"/>
        </div>
    </div>
</div>