<script lang="ts">
    import banner from "../assets/images/banner.png"
    import cv from "../assets/docs/CV - Samuel Rivera.pdf"
    import about from "../assets/images/about.png"
    import blogr from "../assets/images/projects/blogr.png"
    import dinastia from "../assets/images/projects/dinastia.png"
    import loopstudios from "../assets/images/projects/loopstudios.png"
    import space from "../assets/images/projects/space.png"
    import sunnyside from "../assets/images/projects/sunnyside.png"
    import wnews from "../assets/images/projects/w-news.png"
    import contact from "../assets/images/contact.png"
    import Check from "svelte-material-icons/OpenInNew.svelte";

    function scrollToSection() {
        const section = document.querySelector('#contact-beacon');
        section.scrollIntoView({ behavior: 'smooth' });
    }
</script>

<style lang="scss">
    
</style>

<main class="flex flex-col justify-center text-black w-full mx-auto max-w-[1400px]">
    <!--banner-->
    <div class="flex flex-col laptop:flex-row items-center justify-between p-10 mt-10">
        <div class="laptop:w-1/2">
            <img src={banner} alt="banner" class="mx-auto">
        </div>
        <div class="laptop:w-1/2">
            <h2 class="text-6xl text-center laptop:text-left font-bold my-10">Bringing Designs To Life With Seamless Functionality.</h2>
            <p class="text-center laptop:text-justify my-4 text-2xl">As a skilled Full-Stack developer, I craft responsive, innovative and 
                user-friendly applications. Explore my latest projects or download my CV here.
            </p>
            <div class="flex max-laptop:justify-center w-full items-center mx-auto gap-5 my-10">
                <a href={cv} target="_blank">
                    <button class="items-center bg-black text-white p-2.5 px-6 rounded-lg text-lg font-semibold border-2 border-black hover:bg-white hover:text-black">
                        Resume <Check class="inline-block mb-1"/>
                    </button>
                </a>
                <button class="font-bold hover:underline" on:click={scrollToSection}>Contact</button>
            </div>
        </div>
    </div>

    <!--About-->
    <div class="flex flex-col items-center justify-between p-10 mx-auto">
        <div class="flex flex-col laptop:flex-row items-center justify-between">
            <div class="laptop:w-1/2">
                <h2 class="text-6xl text-center laptop:text-justify font-bold mb-10">About Me</h2>
                <p class="text-center laptop:text-justify my-4 text-2xl">Hello, my name is Samuel Rivera, a Full-Stack web developer 
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
        <div class="flex flex-col laptop:flex-row items-center mt-10">
            <div class="laptop:w-1/2 mt-10 laptop:mr-10">
                <h2 class="text-6xl text-center laptop:text-left font-bold mb-10">Skills</h2>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1 border-2 border-black hover:bg-white hover:text-black">HTML5</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1 border-2 border-black hover:bg-white hover:text-black">CSS3</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1 border-2 border-black hover:bg-white hover:text-black">SASS</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1 border-2 border-black hover:bg-white hover:text-black">JavaScript</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1 border-2 border-black hover:bg-white hover:text-black">TypeScript</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1 border-2 border-black hover:bg-white hover:text-black">Node JS</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1 border-2 border-black hover:bg-white hover:text-black">Express</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1 border-2 border-black hover:bg-white hover:text-black">React</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1 border-2 border-black hover:bg-white hover:text-black">Svelte</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1 border-2 border-black hover:bg-white hover:text-black">Bootstrap</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1 border-2 border-black hover:bg-white hover:text-black">Tailwind CSS</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1 border-2 border-black hover:bg-white hover:text-black">Git/GitHub</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1 border-2 border-black hover:bg-white hover:text-black">PostgreSQL</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1 border-2 border-black hover:bg-white hover:text-black">MongoDB</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1 border-2 border-black hover:bg-white hover:text-black">Heroku</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1 border-2 border-black hover:bg-white hover:text-black">AWS S3</p>
                <p class="text-center text-2xl bg-black rounded-full cursor-pointer text-white inline-block w-auto px-4 my-1 border-2 border-black hover:bg-white hover:text-black">AWS Elastic Beanstalk</p>                                                 
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
    <div class="items-center w-full p-10">
        <div class="flex flex-col">
            <h2 class="text-6xl text-center font-bold mb-10">Projects</h2>
            <div class="grid grid-cols-1 tablet:grid-cols-2 laptop:grid-cols-3 desktop:grid-cols-4 gap-6">
                <a href="http://stake-project.s3-website-us-east-1.amazonaws.com/" target="_blank" rel="noopener noreferrer">
                    <div class="bg-gray-100 p-4 shadow rounded hover:bg-gray-300 cursor-pointer">
                        <img src={dinastia} alt="dinastia" class="w-full h-auto">
                        <h3 class="text-2xl mt-4 text-right">Dinastía</h3>
                    </div>
                </a>
                <a href="https://samuelriverab.github.io/sunnyside/" target="_blank" rel="noopener noreferrer">
                    <div class="bg-gray-100 p-4 shadow rounded hover:bg-gray-300 cursor-pointer">
                        <img src={sunnyside} alt="sunnyside" class="w-full h-auto">
                        <h3 class="text-2xl mt-4 text-right">Sunnyside</h3>
                    </div>
                </a>
                <a href="https://samuelriverab.github.io/blogr/" target="_blank" rel="noopener noreferrer">
                    <div class="bg-gray-100 p-4 shadow rounded hover:bg-gray-300 cursor-pointer">
                        <img src={blogr} alt="blogr" class="w-full h-auto">
                        <h3 class="text-2xl mt-4 text-right">Blogr</h3>
                    </div>
                </a>
                <a href="https://samuelriverab.github.io/loopstudios/" target="_blank" rel="noopener noreferrer">
                    <div class="bg-gray-100 p-4 shadow rounded hover:bg-gray-300 cursor-pointer">
                        <img src={loopstudios} alt="loopstudios" class="w-full h-auto">
                        <h3 class="text-2xl mt-4 text-right">Loopstudios</h3>
                    </div>
                </a>
                <a href="https://samuelriverab.github.io/w-news/" target="_blank" rel="noopener noreferrer">
                    <div class="bg-gray-100 p-4 shadow rounded hover:bg-gray-300 cursor-pointer">
                        <img src={wnews} alt="w-news" class="w-full h-auto">
                        <h3 class="text-2xl mt-4 text-right">W-News</h3>
                    </div>
                </a>
                <a href="https://samuelriverab.github.io/space/" target="_blank" rel="noopener noreferrer">
                    <div class="bg-gray-100 p-4 shadow rounded hover:bg-gray-300 cursor-pointer">
                        <img src={space} alt="space" class="w-full h-auto">
                        <h3 class="text-2xl mt-4 text-right">Space</h3>
                    </div>
                </a>
                <!-- Add more project cards with images as needed -->
            </div>
        </div>
    </div>

    <!--Experience-->
    <div class="items-center w-full p-10">
        <div class="flex flex-col">
            <h2 class="text-6xl text-center font-bold mb-10">Experience</h2>
            <div class="relative">
                <div class="flex flex-col space-y-5">
                    <div class="flex flex-col">
                        <div class="absolute mt-1 h-4 w-4 rounded-full bg-gray-500"></div>
                        <div class="flex flex-col ml-6 gap-4">
                            <p class="text-gray-500 text-1xl">June 2022 - Present</p>
                            <h3 class="text-3xl font-semibold">LAB SATOSHI, Medellín, Colombia</h3>
                            <p class="text-2xl text-gray-500 laptop:text-justify">Tasked with the development and maintenance of a responsive and visually appealing website.
                                I also served as a QA Analyst in charge of the execution of periodical and comprehensive testing of client-side
                                applications, ensuring they meet functional requirements, quality standards, and user expectations.
                            </p>
                        </div>
                    </div>
                    <div class="flex flex-col">
                        <div class="absolute mt-1 h-4 w-4 rounded-full bg-gray-500"></div>
                        <div class="flex flex-col ml-6 gap-4">
                            <p class="text-gray-500 text-1xl">August 2021 - February 2022</p>
                            <h3 class="text-3xl font-semibold">CLOWSYSTEMS, Medellín, Colombia</h3>
                            <p class="text-2xl text-gray-500 laptop:text-justify">Participated in the development and maintenance of various responsive and user-friendly
                                web applications, ensuring the writing of clean, efficient, and well-structured code for front-end development 
                                projects.
                            </p>
                        </div>
                    </div>
                    <div class="flex flex-col">
                        <div class="absolute mt-1 h-4 w-4 rounded-full bg-gray-500"></div>
                        <div class="flex flex-col ml-6 gap-4">
                            <p class="text-gray-500 text-1xl">January 2021 - June 2021</p>
                            <h3 class="text-3xl font-semibold">METRO DE MEDELLÍN LTDA, Medellín, Colombia</h3>
                            <p class="text-2xl text-gray-500 laptop:text-justify">Tasked with the development of a visually appealing and user-friendly web application for visualizing and
                                managing a Database and a set of business information through writing of high-quality code based on specific 
                                design specifications, ensuring the successful implementation of required features and functionalities.</p>
                        </div>
                    </div>
                </div>
                <div class="absolute left-1.5 top-2 h-full w-1 bg-gray-500"></div>
            </div>
        </div>
    </div>

    <!--Contact-->
    <div class="items-center w-full p-10">
        <div class="flex flex-col laptop:flex-row items-center">
            <div class="laptop:w-1/2">
                <img src={contact} alt="banner" class="mx-auto my-10">
            </div>
            
            <div class="laptop:w-1/2">
                <h2 id="contact-beacon" class="text-6xl text-center laptop:text-left font-bold mb-10">Contact</h2>
                <p class="text-center laptop:text-justify my-4 text-2xl">If you have any inquiries or would like to discuss a potential collaboration,
                    please feel free to reach out to me. You can contact me via email or phone using the details provided below: <br><br>
                    Email: samuelrivba@gmail.com <br>
                    Phone: +57 3115235240 <br><br>
                    
                    I look forward to hearing from you and will respond to your message as soon as possible. Thank you for your interest!
                </p>
            </div>
        </div>
    </div>
</main>