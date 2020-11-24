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

        h1 {
            font-size: 32px;
            line-height: 43px;
            padding-top: 73px;
            max-width: 700px;
        }
    }
</style>

<div id="start" class="hero-container">
    <div class="hero-content">
        <div>
            <h1>Hello and welcome to my portfolio! <br>My name is Tim and I'm currently a student at Xenters 3D-Technician program.</h1>
        </div>
    </div>
</div>