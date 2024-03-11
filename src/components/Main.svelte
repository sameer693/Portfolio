<script>

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
                <p class="text-base sm:text-lg md:text-xl py-3">
                    My favorite technologies include:
                    <li class=''><span class="text-violet-500 poppins">Web Development:</span><br/>Python(Flask),JS(Svelte),Tailwind CSS,NodeJs</li>                    
                    <li class=''><span class="text-violet-500 poppins">Mobile Development:</span> Dart (Flutter),Firebase</li>
                    <li class=''><span class="text-violet-500 poppins">Machine Learning:</span> Python (Tensorflow, PyTorch)</li> 
                    <li class=''><span class="text-violet-500 poppins">Databases:</span> SQL(Oracle,Mysql,sqlite3), NoSQL</li>
                </p>
                <!--
                    create a link button to get in touch
                -->
                <a href="/contact" target="_blank" class="mx-auto lg:mr-auto sm:text-lg md:text-xl text-base poppins relative overflow-hidden  px-4 py-2  bg-white rounded-full hover:bg-violet-900 duration-200 cursor-pointer">
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
    
</main>
    <slot />