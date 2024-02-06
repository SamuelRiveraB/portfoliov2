<script lang="ts">
    import linkedin from '../assets/images/linkedin.png'
    import github from '../assets/images/github.png'
    import arrow from "../assets/images/arrow.png"
    import logo from "../assets/images/logo2.png"
</script>
  
<style lang="scss">
    button:focus {
        outline: 0;
    }

    .socials {
        z-index: 1;
        display: flex;
        height: 100%;
        position: relative;
        border: none;
        background-color: transparent;
        justify-content: center;
        align-items: center;
        cursor: default;
    }

    .logo {
        display: flex;
        width: 100px;
        height: 100px;
        position: relative;
        border: none;
        border-radius: 50%;
        background-color: #ffffff;
        justify-content: center;
        align-items: center;
        -webkit-box-shadow: 0px 4px 0px 0px rgba(0,0,0,0.1);
        -moz-box-shadow: 0px 4px 0px 0px rgba(0,0,0,0.1);
        box-shadow: 0px 4px 0px 0px rgba(0,0,0,0.1);
    }

    .container {
        z-index: -1;
        width: 100%;
        position: absolute;
        display: flex;
        justify-content: center;
        align-items: center;
        transition: all 0.1s;
        background-color: transparent;
        visibility: hidden;
    }

    .cont-img {
        width: 40px;
        cursor: pointer;
        filter: grayscale(100%) brightness(0);
    }

    .socials:hover .logo-img {
        visibility: hidden;
    }

    .socials:hover .container {
        z-index: 2;
        visibility: visible;
    }

    .cont-img:hover {
        filter: none;
    }

    @keyframes moveUpDown {
        0% {
            transform: translateY(0);
        }
        50% {
            transform: translateY(-10px);
        }
        100% {
            transform: translateY(0);
        }
    }

    .arrow {
        animation: moveUpDown 5s ease-in-out infinite;
    }
</style>

<main>
    <button class="socials hover:hidden">
        <div class="logo">
            <img src={logo} alt="Socials logo" class="h-[70px] mt-5">
        </div>
        <div class="container gap-2">
            <a href="https://www.linkedin.com/in/samuel-rivera-barrientos-38b54317a/" target="_blank" rel="noopener noreferrer">
                <img class="cont-img" src={linkedin} alt="linkedin" />
            </a>
            <a href="https://github.com/SamuelRiveraB" target="_blank" rel="noopener noreferrer">
                <img class="cont-img" src={github} alt="github" />
            </a>
        </div>
    </button>
    <img src={arrow} alt="arrow" class="arrow absolute w-16 top-8 left-full">
</main>