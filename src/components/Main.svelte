<script lang="ts">
    import banner from "../assets/images/banner.png"
    import about from "../assets/images/about.png"
    import foot from "../assets/images/foot.png"
    import blogr from "../assets/images/projects/blogr.png"
    import loopstudios from "../assets/images/projects/loopstudios.png"
    import space from "../assets/images/projects/space.png"
    import sunnyside from "../assets/images/projects/sunnyside.png"
    import wnews from "../assets/images/projects/w-news.png"

    function openNewTab(link: string) {
     window.open(link, '_blank');
    }
</script>
  
<style lang="scss">
    
</style>

<main class="flex flex-col justify-center text-dark w-full mx-auto max-w-[1500px]">
    <!--banner-->
    <div class="flex flex-col laptop:flex-row items-center justify-between p-10 mt-10">
        <div class="laptop:w-1/2">
            <img src={banner} alt="banner" class="mx-auto">
        </div>
        <div class="laptop:w-1/2">
            <h2 class="text-6xl text-center laptop:text-left font-bold my-10">Bringing Designs To Life With Seamless Functionality.</h2>
            <p class="text-center laptop:text-left my-4 text-2xl">As a skilled Full-Stack developer, I craft responsive, innovative and 
                user-friendly applications. Explore my latest projects or download my CV here.
            </p>
            <div class="flex max-laptop:justify-center w-full items-center mx-auto gap-5 my-10">
                <button class="items-center bg-black text-white p-2.5 px-6 rounded-lg text-lg font-semibold">
                    Resume
                </button>
                <a class="text-bold" href="/">Contact</a>
            </div>
        </div>
    </div>
    <!--About-->
    <div class="flex flex-col items-center justify-between p-10 mx-auto">
        <div class="flex flex-col laptop:flex-row items-center justify-between">
            <div class="laptop:w-1/2">
                <h2 class="text-6xl text-center laptop:text-left font-bold mb-10">About Me</h2>
                <p class="text-center laptop:text-left my-4 text-2xl">Hello, my name is Samuel Rivera, a Full-Stack web developer 
                    with a passion for transforming ideas into functional and visually appealing websites. With about 2 years of 
                    experience, I have the unique ability to work with both the front-end and back-end aspects of web development. 
                    From crafting visually appealing and interactive user interfaces to designing and implementing robust server-side
                    logic, I am well-versed in the entire web development stack.<br><br>
                    Being a full stack developer enables me to take a holistic approach to projects, seamlessly integrating front-end
                    and back-end components to deliver cohesive and functional web applications. I pride myself on my ability to handle
                    both client-side and server-side challenges, providing end-to-end solutions that meet the needs of users and clients
                    alike.<br><br>
                    I specialize in creating user-friendly interfaces and ensuring responsive experiences across devices. Whether it's
                    crafting clean and efficient code, integrating frameworks like React and Svelte, or working with Back-end technologies
                    such as Node.js and databases like MongoDB, I bring my commitment to deliver high-quality solutions. I am thrilled at the
                    opportunity to work with you and be part of your team.
                </p>
            </div>
            <div class="laptop:w-1/2">
                <img src={about} alt="img" class="mx-auto">
            </div>
        </div>
        <div class="flex flex-col laptop:flex-row items-center justify-between mt-10">
            <div class="laptop:w-1/2 mt-10 laptop:mr-10">
                <h2 class="text-6xl text-center laptop:text-left font-bold mb-10">Skills</h2>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1">HTML5</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1">CSS3</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1">SASS</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1">JavaScript</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1">TypeScript</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1">Node JS</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1">Express</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1">React</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1">Svelte</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1">Bootstrap</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1">Tailwind CSS</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1">Git/GitHub</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1">PostgreSQL</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1">MongoDB</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1">Heroku</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1">AWS S3</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1">AWS Elastic Beanstalk</p>                                                 
            </div>
            <div class="w-full laptop:w-1/2 pb-10 mt-10">
                <h2 class="text-6xl text-center laptop:text-left font-bold mb-10">Languages</h2>
                <p class="text-2xl my-2">Spanish</p>
                <div class="relative w-full h-5 bg-gray-200 rounded-full">
                    <div class="absolute top-0 left-0 h-full bg-black rounded-full w-full"></div>
                </div>
                <p class="text-2xl my-2">English</p>
                <div class="relative w-full h-5 bg-gray-200 rounded-full">
                    <div class="absolute top-0 left-0 h-full bg-black rounded-full w-[85%]"></div>
                </div>
            </div>
        </div>
    </div>
    <!--Projects-->
    <div class="items-center justify-between w-full p-10">
        <div class="flex flex-col">
            <h2 class="text-6xl text-center font-bold mb-10">Projects</h2>
            <div class="grid grid-cols-1 tablet:grid-cols-2 laptop:grid-cols-3 desktop:grid-cols-4 gap-6">
                <div on:click={() => openNewTab("https://samuelriverab.github.io/sunnyside/")} on:keydown={() => this.click} class="bg-gray-100 p-4 shadow rounded hover:bg-gray-300 cursor-pointer">
                    <img src={sunnyside} alt="sunnyside" class="w-full h-auto">
                    <h3 class="text-2xl mt-4 text-right">Sunnyside</h3>
                </div>
                <div on:click={() => openNewTab("https://samuelriverab.github.io/blogr/")} on:keydown={() => this.click} class="bg-gray-100 p-4 shadow rounded hover:bg-gray-300 cursor-pointer">
                    <img src={blogr} alt="blogr" class="w-full h-auto">
                    <h3 class="text-2xl mt-4 text-right">Blogr</h3>
                </div>
                <div on:click={() => openNewTab("https://samuelriverab.github.io/loopstudios/")} on:keydown={() => this.click} class="bg-gray-100 p-4 shadow rounded hover:bg-gray-300 cursor-pointer">
                    <img src={loopstudios} alt="loopstudios" class="w-full h-auto">
                    <h3 class="text-2xl mt-4 text-right">Loopstudios</h3>
                </div>
                <div on:click={() => openNewTab("https://samuelriverab.github.io/w-news/")} on:keydown={() => this.click} class="bg-gray-100 p-4 shadow rounded hover:bg-gray-300 cursor-pointer">
                    <img src={wnews} alt="w-news" class="w-full h-auto">
                    <h3 class="text-2xl mt-4 text-right">W-News</h3>
                </div>
                <div on:click={() => openNewTab("https://samuelriverab.github.io/space/")} on:keydown={() => this.click} class="bg-gray-100 p-4 shadow rounded hover:bg-gray-300 cursor-pointer">
                    <img src={space} alt="space" class="w-full h-auto">
                    <h3 class="text-2xl mt-4 text-right">Space</h3>
                </div>
                <!-- Add more project cards with images as needed -->
            </div>
        </div>
    </div>
    <!--Experience-->
    <div class="items-center justify-between w-full p-10">
        <div class="flex flex-col laptop:flex-row">
            <div class="">
                <h2 class="text-6x1 text-left">Experience</h2>
                <div class="relative">
                    <div class="flex flex-col space-y-4">
                      <div class="flex items-start">
                        <div class="h-4 w-4 rounded-full bg-blue-500"></div>
                        <div class="ml-4">
                          <h3 class="text-lg font-semibold">Event 1</h3>
                          <p class="text-gray-500">Description of Event 1</p>
                        </div>
                      </div>
                      <div class="flex items-start">
                        <div class="h-4 w-4 rounded-full bg-blue-500"></div>
                        <div class="ml-4">
                          <h3 class="text-lg font-semibold">Event 2</h3>
                          <p class="text-gray-500">Description of Event 2</p>
                        </div>
                      </div>
                      <div class="flex items-start">
                        <div class="h-4 w-4 rounded-full bg-blue-500"></div>
                        <div class="ml-4">
                          <h3 class="text-lg font-semibold">Event 3</h3>
                          <p class="text-gray-500">Description of Event 3</p>
                        </div>
                      </div>
                    </div>
                    <div class="absolute left-4 top-0 h-full w-1 bg-blue-500"></div>
                  </div>
            </div>
        </div>
    </div>
    <!--Contact-->
    <div class="items-center justify-between w-full p-10">
        <div class="flex flex-col laptop:flex-row">
            <div class="">
                <h2 class="text-6x1 text-left">Contact</h2>
                <p class="my-4 text-base font-medium">As a skilled full stack developer, I craft responsive, innovative and user-friendly applications. Explore my latest projects or download my CV here.</p>
            </div>
            <div class="">
                <img src={banner} class="w-full h-auto" alt="img">
            </div>
        </div>
    </div>
    <!--Contact-->
    <div class="items-center justify-between w-full p-10">
        <div class="flex flex-col laptop:flex-row">
            <div class="">
                <h2 class="text-6x1 text-left">Footer</h2>
                <p class="my-4 text-base font-medium">As a skilled full stack developer, I craft responsive, innovative and user-friendly applications. Explore my latest projects or download my CV here.</p>
            </div>
            <div class="">
                <img src={foot} class="w-full h-auto" alt="img">
            </div>
        </div>
    </div>
</main>