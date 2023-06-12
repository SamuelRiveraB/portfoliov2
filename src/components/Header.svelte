<script lang="ts">
    import Socials from './Socials.svelte';
</script>

<style lang="scss">

</style>

<header class="flex fixed w-full h-[50px] justify-center items-center shadow bg-white z-50">
    <div class="absolute">
        <Socials/>
    </div>
    <div class="flex mx-auto items-center w-full max-w-[1400px] p-2 tablet:p-10">
        <a href="/">
            <h2 class="cursor-pointer text-bold text-left text-[30px]">Samuel<span class="text-purple-500">.</span></h2>
        </a>
    </div>
</header>