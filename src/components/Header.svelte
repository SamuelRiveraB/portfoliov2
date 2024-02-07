<script lang="ts">
    import Socials from './Socials.svelte';
    import logo from "../assets/images/logo.png"
</script>

<style lang="scss">

</style>

<header class="flex fixed w-full h-[50px] justify-center items-center shadow bg-white z-50">
    <!-- <div class="absolute">
        <Socials/>
    </div> -->
    <div class="flex mx-auto items-center justify-between w-full max-w-[1400px] p-2 tablet:p-10">
        <a href="/">
            <img src={logo} alt="Header logo" class="h-7">
        </a>
        <ul class="hidden tablet:flex gap-10 font-bold">
            <li class="cursor-pointer hover:text-myGreen"><a href="/">About</a></li>
            <li class="cursor-pointer hover:text-myGreen">Skills</li>
            <li class="cursor-pointer hover:text-myGreen">Projects</li>
            <li class="cursor-pointer hover:text-myGreen">Contact</li>
        </ul>
    </div>
</header>