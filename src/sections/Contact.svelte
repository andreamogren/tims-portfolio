<style lang="scss">
    @import '../../public/assets/variables';

    $logo-size: 80px;

    .contact-container {
        @include container-styles;

        h2 {
            @include h2-styles;
        }

        .logos {
            margin: 0 auto; 
            display: flex;
            align-items: center;
            justify-content: center;
        }
        .logo > img {
            max-width: $logo-size;
            height: $logo-size;
            transition: 0.3s;
            padding: $base-padding;

            &:hover {
                transform: scale(1.1); 
            }
        }
    }


</style>

<div id="contact" class="contact">
    <div class="contact-container">
        <h2>Contact</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
        <div class="logos">
            <a class="logo" href="mailto:timhellberg@gmail.com"><img src="./assets/email.svg" alt="Email"/></a>
            <a class="logo" href="https://www.linkedin.com/in/tim-hellberg-5b7647196/"><img src="./assets/linkedin.png" alt="LinkedIn profile"/></a>
        </div>
    </div>
</div>