<script lang="ts">
    import banner from "../assets/images/banner_photo.png"
    import cv from "../assets/docs/CV - Samuel Rivera.pdf"
    import about from "../assets/images/about_photo.png"
    import blogr from "../assets/images/projects/blogr.png"
    import dinastia from "../assets/images/projects/dinastia.png"
    import loopstudios from "../assets/images/projects/loopstudios.png"
    import pongalong from "../assets/images/projects/pongalong.png"
    import space from "../assets/images/projects/space.png"
    import sunnyside from "../assets/images/projects/sunnyside.png"
    import wnews from "../assets/images/projects/w-news.png"
    import Check from "svelte-material-icons/OpenInNew.svelte";
    import linkedin from '../assets/images/linkedin.png'
    import github from '../assets/images/github.png'

    function scrollToSection() {
        const section = document.querySelector('#contact');
        section.scrollIntoView({ behavior: 'smooth' });
    }
</script>

<style lang="scss">

</style>

<main class="flex flex-col justify-center text-black w-full mx-auto">
    <!--banner-->
    <div class="flex justify-center items-center h-[100vh] min-h-[700px] laptop:p-10">
        <div class="w-full h-full flex flex-col-reverse laptop:flex-row items-center justify-center">
            <div class="">
                <h2 class="text-5xl text-center laptop:text-left font-bold my-10">Hi, my name is <span class="text-myGreen">Samuel</span></h2>
                <p class="text-center laptop:text-justify my-4 text-2xl">I'm a Full Stack Web Developer based in Medellín, Colombia.
                </p>
                <div class="flex max-laptop:justify-center w-full items-center mx-auto gap-5 my-10">
                    <a href={cv} target="_blank">
                        <button class="transition items-center bg-black text-white p-2.5 px-6 rounded-lg text-lg font-semibold border-2 border-black hover:bg-white hover:text-black">
                            Resumé <Check class="inline-block mb-1"/>
                        </button>
                    </a>
                    <button class="font-bold hover:text-myGreen" on:click={scrollToSection}>Contact</button>
                </div>
            </div>
            <div class="relative w-[40%] laptop:w-[30%]">
                <a  href="https://www.linkedin.com/in/samuel-rivera-barrientos-38b54317a/" target="_blank"  rel="noopener noreferrer">
                    <img src={banner} alt="Banner" class="mx-auto w-full laptop:w-[70%]">
                    <img src={linkedin} alt="Banner Linkedin" class="absolute w-[15%] bottom-1 right-5">
                </a>
            </div>
        </div>
    </div>

    <!--About-->
    <div class="flex flex-col items-center justify-between p-20 mx-auto bg-myGreen w-full py-20">
        <div class="flex flex-col laptop:flex-row items-center justify-between">
            <div class="max-w-[1140px]">
                <h2 class="text-6xl text-center font-bold mb-10 text-white">About Me</h2>
                <div class="flex flex-col laptop:flex-row items-center gap-10 laptop:gap-0">
                    <div class="w-full flex justify-center items-center">
                        <img src={about} alt="img" class="w-[50%] ">
                    </div>
                    <p class="text-center laptop:text-justify text-xl text-white w-full">I'm a Full-Stack Developer with a passion for transforming ideas into functional and visually appealing websites. I have a comprehensive grasp of both front-end and back-end development. I pride myself with my ability to learn things quickly and interest in enhancing my skillset, and I'm certain that a can contribute effectively to any Web Development team.
                    </p>
                </div>
            </div>
        </div>
    </div>

    <!-- Skills -->
    <div class="flex flex-col items-center justify-between p-20 w-[100vw]">
        <div class="max-w-[1140px] w-full">
            <h2 class="text-6xl text-center font-bold mb-10">Skills</h2>
            <div class="flex flex-col laptop:flex-row gap-10 justify-center">
                <div class="rounded-md shadow-md grow">
                    <div class="bg-myGreen rounded-t-md text-white px-20 py-5 text-2xl">
                        <h3 class="text-center">Front End</h3>
                    </div>
                    <div class="flex flex-col gap-5 p-10 text-xl text-center">
                        <p>HTML5</p>
                        <p>CSS3</p>
                        <p>SASS</p>
                        <p>Javascript</p>
                        <p>Typescript</p>
                        <p>React</p>
                        <p>NextJS</p>
                        <p>Svelte</p>
                        <p>TailwindCSS</p>
                        <p>Bootstrap</p>
                    </div>
                </div>

                <div class="rounded-md shadow-md grow">
                    <div class="bg-myGreen rounded-t-md text-white px-20 py-5 text-2xl">
                        <h3 class="text-center">Back End</h3>
                    </div>
                    <div class="flex flex-col gap-5 p-10 text-xl text-center">
                        <p>NodeJS</p>
                        <p>Express</p>
                        <p>Postgres</p>
                        <p>MongoDB</p>
                        <p>Restful APIs</p>
                        <p>Python</p>
                    </div>
                </div>

                <div class="rounded-md shadow-md grow">
                    <div class="bg-myGreen rounded-t-md text-white px-20 py-5 text-2xl">
                        <h3 class="text-center">Other</h3>
                    </div>
                    <div class="flex flex-col gap-5 p-10 text-xl text-center">
                        <p>Git</p>
                        <p>Github</p>
                        <p>Vercel</p>
                        <p>SCRUM</p>
                        <p>VSCode</p>
                        <p>AWS</p>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!--Projects-->
    <div class="flex flex-col items-center justify-between p-20 w-[100vw] bg-myGreen">
        <div class="max-w-[1140px] w-full">
            <h2 class="text-6xl text-center font-bold mb-10 text-white">Projects</h2>
            <div class="grid grid-cols-1 tablet:grid-cols-2 laptop:grid-cols-3 gap-6">
                
                <a href="https://samuelriverab.github.io/pongalong/" target="_blank" rel="noopener noreferrer">
                    <div class="bg-gray-100 p-4 shadow rounded hover:bg-gray-300 cursor-pointer">
                        <div class="bg-gray-300 w-full h-40 flex justify-center items-center">
                            <img src={pongalong} alt="Pongalong" class="h-full object-cover">
                        </div>
                        <h3 class="text-2xl mt-4 text-right">Bad UIs - Pongalong</h3>
                    </div>
                </a>

                <a href="http://stake-project.s3-website-us-east-1.amazonaws.com/" target="_blank" rel="noopener noreferrer">
                    <div class="bg-gray-100 p-4 shadow rounded hover:bg-gray-300 cursor-pointer">
                        <div class="bg-gray-300 w-full h-40 flex justify-center items-center">
                            <img src={dinastia} alt="Dinastia" class="h-full object-cover">
                        </div>
                        <h3 class="text-2xl mt-4 text-right">Dinastía</h3>
                    </div>
                </a>

                <a href="https://samuelriverab.github.io/sunnyside/" target="_blank" rel="noopener noreferrer">
                    <div class="bg-gray-100 p-4 shadow rounded hover:bg-gray-300 cursor-pointer">
                        <div class="bg-gray-300 w-full h-40 flex justify-center items-center">
                            <img src={sunnyside} alt="Sunnyside" class="h-full object-cover">
                        </div>
                        <h3 class="text-2xl mt-4 text-right">Sunnyside</h3>
                    </div>
                </a>

                <a href="https://samuelriverab.github.io/blogr/" target="_blank" rel="noopener noreferrer">
                    <div class="bg-gray-100 p-4 shadow rounded hover:bg-gray-300 cursor-pointer">
                        <div class="bg-gray-300 w-full h-40 flex justify-center items-center">
                            <img src={blogr} alt="Blogr" class="h-full object-cover">
                        </div>
                        <h3 class="text-2xl mt-4 text-right">Blogr</h3>
                    </div>
                </a>

                <a href="https://samuelriverab.github.io/loopstudios/" target="_blank" rel="noopener noreferrer">
                    <div class="bg-gray-100 p-4 shadow rounded hover:bg-gray-300 cursor-pointer">
                        <div class="bg-gray-300 w-full h-40 flex justify-center items-center">
                            <img src={loopstudios} alt="Loopstudios" class="h-full object-cover">
                        </div>
                        <h3 class="text-2xl mt-4 text-right">Loopstudios</h3>
                    </div>
                </a>

                <a href="https://samuelriverab.github.io/w-news/" target="_blank" rel="noopener noreferrer">
                    <div class="bg-gray-100 p-4 shadow rounded hover:bg-gray-300 cursor-pointer">
                        <div class="bg-gray-300 w-full h-40 flex justify-center items-center">
                            <img src={wnews} alt="W News" class="h-full object-cover">
                        </div>
                        <h3 class="text-2xl mt-4 text-right">W-News</h3>
                    </div>
                </a>

                <a href="https://samuelriverab.github.io/space/" target="_blank" rel="noopener noreferrer">
                    <div class="bg-gray-100 p-4 shadow rounded hover:bg-gray-300 cursor-pointer">
                        <div class="bg-gray-300 w-full h-40 flex justify-center items-center">
                            <img src={space} alt="space" class="h-full object-cover">
                        </div>
                        <h3 class="text-2xl mt-4 text-right">Space</h3>
                    </div>
                </a>

                <!-- Add more project cards with images as needed -->
            </div>
        </div>
    </div>

    <!--Experience-->
    <div class="items-center w-full p-10 pb-20 laptop:p-20">
        <div class="flex flex-col">
            <h2 class="text-6xl text-center font-bold mb-10">Experience</h2>
            <div class="relative">
                <div class="flex flex-col space-y-5">
                    <div class="flex flex-col">
                        <div class="absolute mt-1 h-4 w-4 rounded-full bg-gray-500"></div>
                        <div class="flex flex-col ml-6 gap-4">
                            <p class="text-gray-500 text-1xl">June 2022 - November 2023</p>
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
    <div id="contact"></div>
    <div class="flex flex-col items-center justify-between p-10 laptop:p-20 w-[100vw] bg-myGreen">
        <div class="max-w-[1140px] w-full">
            <h2 class="text-6xl text-center font-bold mb-10 text-white">Contact</h2>
            <div class="flex flex-col laptop:flex-row gap-10 justify-center">

                <div class="rounded-md shadow-md grow laptop:w-1/3 min-h-[110px]">
                    <a href="mailto:samuelrivba@gmail.com">
                        <div class="rounded-md shadow-md bg-white flex items-center h-full min-h-[110px]">
                            <div class="rounded-md px-20 py-5 flex justify-center items-center text-xl w-full">
                                <h3 class="text-center">Email: samuelrivba@gmail.com</h3>
                            </div>
                        </div>
                    </a>
                </div>

                <div class="rounded-md shadow-md grow laptop:w-1/3">
                    <a href="https://www.linkedin.com/in/samuel-rivera-barrientos-38b54317a/" target="_blank" rel="noopener noreferrer">
                        <div class="rounded-md shadow-md grow bg-white flex items-center justify-center h-full">
                            <div class="rounded-md px-20 py-5 flex justify-center items-center w-full">
                                <img src={linkedin} alt="Linkedin" class="w-[70px]">
                            </div>
                        </div>
                    </a>
                </div>

                <div class="rounded-md shadow-md grow laptop:w-1/3">
                    <a href="https://github.com/SamuelRiveraB" target="_blank"  rel="noopener noreferrer">
                        <div class="rounded-md shadow-md grow bg-white flex items-center justify-center h-full">
                            <div class="rounded-md px-20 py-5 flex justify-center items-center w-full">
                                <img src={github} alt="GitHub" class="w-[70px]"/>
                            </div>
                        </div>
                    </a>
                </div>
            </div>
        </div>
    </div>
</main>