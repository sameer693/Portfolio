<script>
    /**
     * @type {{ href: any; title: any; description: any; icon: any; }}
     */
     export let step;
    export let index;
</script>

<!--
    let steps=[
            {title:"Bus Rapid Transit (BRT) Ticketing System App",icon:"bus",description:"I have worked on this web development project using Python(flask),Jinja,sqlite3, gunicorn and ngrok for hosting"},
            {title:"IIIT-NR app",icon:"mobile",description:"I have worked on official IIIT-NR mobile applications using Flutter, NodeJS and Firebase ."},
            {title:"Political speech analysis",icon:"machine-learning",description:"I have worked on  machine learning projects using Python(SpaCy) and Jupyter notebooks."},
            {title:"project battler game website",icon:"web",description:"I have worked on this web development project using Python(flask),Jinja and sqlite3"}
        ];
-->

<a href={step.href} target="_blank" class="relative p-4 sm:p-6  md:pd-8  flex flex-col gap-6  rounded-lg border border-solid border-violet-700  text-center group cursor-pointer hover:border-violet-400 shadow-md shadow-violet-500 duration-200">
    
      <div class=" absolute top-0 left-1/2 transform -translate-x-1/2 -translate-y-1/2 gap-2 ">
        <i class="{step.icon} text-4xl"></i>
      </div>
    <div class="flex flex-col gap-2">
        <h1 class="text-2xl font-bold text-violet-400">{step.title}</h1>
        <p class="text-base">{step.description}</p>
    </div>
</a>
