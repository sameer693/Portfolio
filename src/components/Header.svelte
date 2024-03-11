<script>
    /**
     * @type {number}
     */
     export let y;
    let tabs=[
        {name:"Projects",href:"/",link:"/projects"},
        {name:"About",href:"/about",link:"/about"},
    ];
</script>

<header class={'sticky z-[10] shadow-lg  shadow-purple-500/50  top-0  duration-200 flex items-center justify-between border border-solid'+(y>0?" py-4 bg-slate-950  border-b-violet-950":" py-6 bg-transparent border-transparent")} >
    <a href="/" class="flex items-center gap-2">
    <h1 class="font-medium ml-2  ">
        <span class="bg-gradient-to-r  from-indigo-500 via-purple-500 to-pink-500 bg-clip-text text-transparent font-extrabold poppins">Sameer Yadav</span>
    </h1>
    </a>
    <div class="sm:flex items-center gap-4 hidden">
            {#each tabs as tab,index}
            <a href={tab.link} class=" duration-200 hover:text-violet-700">
                <p class="mx-2">{tab.name}</p>
            </a>
            {/each}
    </div>
    <!-- Get in touch -->
    <a href="/contact" class="px-4 py-2 shadow-lg shadow-indigo-500/50  bg-white text-black rounded-full hover:bg-violet-900 duration-200">
        <h4 class="relative z-[9] bg-gradient-to-r from-indigo-500 via-purple-500 to-pink-500 bg-clip-text text-transparent font-bold poppins">Get in touch</h4>
    </a>
</header>