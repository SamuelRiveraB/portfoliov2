<script lang="ts">
    import hire from "../assets/images/hire.png"
    import foot from "../assets/images/foot.png"

    const currentYear = new Date().getFullYear();
</script>

<style lang="scss">
    
</style>

<footer class="flex bottom-0 w-full justify-center items-center bg-white p-10">
    <div class="flex flex-col justify-center items-center gap-3">
        <a href="/">
            <h2 class="cursor-pointer text-bold text-left text-[30px]">Samuel<span class="text-purple-500">.</span></h2>
        </a>
        <p class="text-2xl justify-center">
            Resources provided by: <a href="https://www.glazestock.com/" target="_blank" rel="noopener noreferrer" class="underline">Glaze</a>
            | <a href="https://www.freepik.com/" target="_blank" rel="noopener noreferrer" class="underline">Freepik</a>
        </p>
        <p>
            © {currentYear} Samuel. | All rights reserved.
        </p>
    </div>
    <!--<img src={foot} alt="foot" class="absolute right-0 w-[120px] mt-[100px]">-->
</footer>