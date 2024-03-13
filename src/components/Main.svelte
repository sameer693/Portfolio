<script>
    import Step from "./Step.svelte";
    let steps=[
                {title:"IIIT-NR app",icon:"fa-solid fa-brands fa-google-play",description:"I have worked on official IIIT-NR mobile applications using Flutter, NodeJS and Firebase .",href:"https://play.google.com/store/apps/details?id=com.iiitnr.app"},
                {title:"Bus Rapid Transit (BRT) Ticketing System App",icon:"bus",description:"I have worked on this web development project using Python(flask),Jinja,sqlite3, gunicorn and ngrok for hosting", href: "https://example.com"},
                {title:"Political speech analysis",icon:"fa-solid fa-brands fa-python",description:"I have worked on  machine learning projects using Python(SpaCy) and Jupyter notebooks.", href: "https://example.com"},
                {title:"project battler game website",icon:"web",description:"I have worked on this web development project using Python(flask),Jinja and sqlite3", href: "https://example.com"}
            ];
    let benifts=[
        {title:"Student",description:"I'm a student at IIIT-NR, currently pursuing my B.Tech in Computer Science and Engineering."},
        {title:"IIITNR App Admin",description:"I'm also currently working as the IIIT-NR app admin and managing the gatepass and various services."},
        {title:"Full Stack Developer",description:"I'm a full-stack developer, proficient in Python, JavaScript, Dart, C, and C++, with a passion for crafting web and mobile solutions."},
        {title:"Ml Enthusiast",description:"I have a keen interest in exploring machine learning, AI and data science."}
    ];
</script>

<main class="flex flex-1 flex-col p-4">
    <section id="intro page" class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14 ">
        <!--
            create a div with a class of flex and justify-center lg:text-left gap-6 md:gap-8 lg:gap-10
        -->
        <div class="flex flex-col justify-center lg:text-left gap-6 md:gap-8 lg:gap-10">
            <div class="flex flex-col justify-center">
                <h1 class="text-4xl font-bold ">Hi! I'm <span class="bg-gradient-to-r from-indigo-500 via-purple-500 to-pink-500 bg-clip-text text-transparent poppins">Sameer Yadav</span>
                <br/>Full stack <span class=" text-violet-500 poppins">Developer !</span> 
                </h1>
                <p class="text-base sm:text-lg md:text-xl py-6 ">
                    My favorite technologies include:
                    <li class=''><span class="text-violet-500 poppins">Web Development:</span><br/>Python(Flask),JS(Svelte),Tailwind CSS,NodeJs</li>                    
                    <li class=''><span class="text-violet-500 poppins">Mobile Development:</span> Dart (Flutter),Firebase</li>
                    <li class=''><span class="text-violet-500 poppins">Machine Learning:</span> Python (Tensorflow, PyTorch)</li> 
                    <li class=''><span class="text-violet-500 poppins">Databases:</span> SQL(Oracle,Mysql,sqlite3), NoSQL</li>
                </p>
                <!--
                    create a link button to get in touch
                -->
                <a href="/contact" target="_blank" class="mx-auto   lg:mr-auto sm:text-lg md:text-xl text-base poppins relative overflow-hidden  px-4 py-2  bg-white rounded-full hover:bg-violet-900 duration-200 cursor-pointer">
                    <div class="absolute top-0 left-0 w-full h-full opacity-20  group-hover:translate-x-full duration-200"/>
                    <h4 class="relative z-[9] bg-gradient-to-r from-indigo-500 via-purple-500 to-pink-500 bg-clip-text text-transparent font-bold poppins">Get in touch <span class="ml-2">&#8594;</span>
                    </h4>
                </a>
            </div>
            
        </div>    
        <div class="justify-center relative grid place-items-center">
            <img src="/images/profile.png" alt="Sameer Yadav" class="object-cover z-[2] max-h-[72vh]" />
          </div>
         
    </section>

    <!--
        create a section with a class of grid and grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14
        for the projects

    -->
    <section id="projects" class="py-1 lg:py-10 flex flex-col ">
        <div class="flex flex-col text-center gap-6">            
            <h1 class="text-4xl font-bold ">MY Projects</h1>    
            <p class="text-base sm:text-lg md:text-xl">
            Want to see some of my work? Here are a few projects I've worked on recently.
            </p>        
            <a href="/projects" class="mx-auto  lg:mr-auto sm:text-lg md:text-xl text-base poppins relative overflow-hidden  px-4 py-2  bg-white rounded-full hover:bg-violet-900 duration-200 cursor-pointer">
                <div class="absolute top-0 left-0 w-full h-full opacity-20  group-hover:translate-x-full duration-200"/>
                <h4 class="relative z-[9] bg-gradient-to-r from-indigo-500 via-purple-500 to-pink-500 bg-clip-text text-transparent font-bold poppins">View Projects <span class="ml-2">&#8594;</span>
                </h4>
            </a>
        </div>  
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-6 md:gap-8 lg:gap-10 py-8" >
            {#each steps as step,index}
                <Step {step} index={index}/>
            {/each}
        </div>  
        
    </section>
    
    <!--
        section for the about me
        contains a bit about me
        
    -->
    <section id="about" class="py-1 lg:py 10 flex flex-col ">
        <!--
            a ray of light effect
        -->
        <div class="flex flex-col text-center gap-6 relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-500 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-400 py-4">        
            <h4 class="text-lg sm:text-xl md:text-2xl">Want to Know more?</h4>
            <h2 class="text-3xl font-semibold ">A bit  <span class="text-violet-500 poppins">About </span>Me</h2>
            <table class="">
                {#each benifts as benifit}
                    <tr>
                        <td class="p-3 text-slate-500 font-semibold">{benifit.title}</td>
                        <td class="p-3">{benifit.description}</td>
                    </tr>
                {/each}
            </table>       
            <p class="text-base sm:text-lg md:text-xl">
                My skills
            </p>
                
            <table class="text-base sm:text-lg md:text-xl rounded-md shadow-md overflow-hidden mt-6">
                <thead class="bg-slate-400">
                  <tr>
                    <th class="p-3 font-bold">Skill</th>
                    <th class="p-3 font-bold">Description</th>
                  </tr>
                </thead>
                <tbody>
                  <tr>
                    <td class="p-3">Dedication</td>
                    <td class="p-3">Committed to achieving goals and delivering high-quality work.</td>
                  </tr>
                  <tr>
                    <td class="p-3">Hardworking</td>
                    <td class="p-3">Willing to put in the effort and go the extra mile to ensure success.</td>
                  </tr>
                  <tr>
                    <td class="p-3">Persistence</td>
                    <td class="p-3">Resilient in the face of challenges, consistently working towards solutions.</td>
                  </tr>
                  <tr>
                    <td class="p-3">Time Management</td>
                    <td class="p-3">Effective organization and allocation of time to maximize productivity.</td>
                  </tr>
                  <tr>
                    <td class="p-3">Communication</td>
                    <td class="p-3">Strong interpersonal skills, ensuring clear and effective communication.</td>
                  </tr>
                  <!-- Add more rows for additional skills -->
                </tbody>
              </table>
        </div>
    </section>

    
</main>
    <slot />