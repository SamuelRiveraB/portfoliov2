<script lang="ts">
    import logo from "../assets/images/logo.png"

    const currentYear = new Date().getFullYear();
</script>

<style lang="scss">
    
</style>

<footer class="flex bottom-0 w-full justify-center items-center p-10">
    <div class="flex flex-col justify-center items-center gap-3">
        <a href="/">
            <img src={logo} alt="Logo" class="w-40">
        </a>
        <p class="mt-2 text-xl justify-center">
            Resources provided by: <a href="https://www.glazestock.com/" target="_blank" rel="noopener noreferrer" class="underline">Glaze</a>
            | <a href="https://www.freepik.com/" target="_blank" rel="noopener noreferrer" class="underline">Freepik</a > | <a href="https://www.canva.com/p/rayhanstudio/"  target="_blank" rel="noopener noreferrer" class="underline">@rayhanstudio</a>
        </p>
        <p>
            © {currentYear} <span class="text-myGreen font-bold">Samuel</span> | All rights reserved.
        </p>
    </div>
    <!--<img src={foot} alt="foot" class="absolute right-0 w-[120px] mt-[100px]">-->
</footer>