<script>
    import Step from "./Step.svelte";

    let steps = [
        {
            name: "Robotics",
            icon: "fa-solid fa-tractor",
            description:"",
        },
        {
            name: "AI & Automation",
            icon: "fa-solid fa-coins",
            description: "",
        },
        {
            name: "Innovation",
            icon: "fa-solid fa-lightbulb",
            description: "",
        },
    ];

    let benefits = [
        {
        name: "a fast learner",
        description:
            "I thrive on challenges and am quick to adapt to new tools, technologies, and environments. My ability to pick up new skills and knowledge allows me to contribute meaningfully and stay ahead in a fast-paced and ever-evolving industry.",
    },
    {
        name: "passionate about making a difference",
        description:
            "I am deeply driven by the desire to create impactful solutions that improve lives, solve real-world problems, and make a lasting difference. Whether through technology, design, or collaboration, my work is fueled by a commitment to positive change.",
    },
    {
        name: "a team player",
        description:
            "I believe that great accomplishments are rarely achieved alone. I thrive in collaborative environments, where I can contribute, support, and learn from my teammates, ensuring the success of the team as a whole.",
    },
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <section
        id="introPage"
        class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
    >
        <div
            class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10"
        >
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hello! My Name is <br/> <span class="poppins text-violet-400">Garab</span> Dorji <br/> and I am a 
                <br />Mechatronics
                <p></p>
                <span class="poppins text-violet-400">Engineer</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                <strong>
                    Mechatronics Engineer   <span class="poppins text-violet-400">|</span>   MSc(Eng). Robotics   <span class="poppins text-violet-400">|</span>   Founder   <span class="poppins text-violet-400">|</span>   UNSW Alumni   <span class="poppins text-violet-400">|</span>  R & D Engineer  <span class="poppins text-violet-400">|</span>   Fullstack Developer   <span class="poppins text-violet-400">|</span>   Automation   <span class="poppins text-violet-400">|</span>   Agile   <span class="poppins text-violet-400">|</span>   AI   <span class="poppins text-violet-400">|</span>    RPA   <span class="poppins text-violet-400">|</span>   SCADA       
                </strong>
            </p>
            
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img
                src={"images/profile.png"}
                alt="Zetane Engine"
                class="object-cover z-[2] max-h-[70vh]"
            />
        </div>
    
    </section>
    <section class="py-20 lg:py-32 flex flex-col gap-24" id="projects">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:text-2xl">
                Curious about my work?
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                More than happy to <span class="poppins text-violet-400">share</span>
            </h3>
        </div>
        <a
            href="https://www.linkedin.com/posts/leaderbrandproduce_the-future-of-farming-is-here-our-engineering-activity-7261833821791109121-B2XC?utm_source=combined_share_message&utm_medium=member_desktop_web"
            target="_blank"
            class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200"
        >
            <i class="fa-regular fa-circle-play" />
            <p>Watch this video</p>
        </a>
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <Step step={steps[0]}>
                <p>
                    Maintained and Co-Developed <strong
                    class="text-violet-400"
                    > autonomous ground vehicles </strong
                >  for harvesting spinach and rocket leaves as well as performed
                <strong
                    class="text-violet-400"
                    > Research Engineer duties </strong
                > 
                  and developed AI solutions for  <strong
                  class="text-violet-400"
                  > detecting spinach leaves’ moisture levels </strong
              >  

                </p>
                
            </Step>
            <Step step={steps[1]}>
                <p>

                    Developed RPA systems that automated <strong
                    class="text-violet-400"> 70% of procurement work </strong
                > for the engineering department as well as discovered <strong class="text-violet-400">3-year expenditure trends</strong
                    > from invoices with OCR
                    
                </p>
            </Step>
            <Step step={steps[2]}>
                <p>
                    Have been a part of many startup endeavors in 
                     <strong class="text-violet-400"
                        >Bhutan</strong
                    > as well as other countries focused on  innovative methods to improve the citizen's quality of life 
                   
                </p>
            </Step>
        </div>
    </section>
    <section
        id="about"
        class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
    >
        <!-- <div class="z-[-1] bg-violet-950 w-screen left-1/2 -translate-x-1/2 top-0 h-full absolute"> </div> -->
        <div
            class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
        >
    
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                A bit <span class="poppins text-violet-400">about</span> me.
            </h3>
        </div>
        <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
            I am . . .
        </p>
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
                
                <div class="flex gap-6 sm:gap-8">
                    <p
                        class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"
                    >
                        0{index + 1}
                    </p>
                    <div class="flex flex-col gap-6 sm:gap-8">
                        <h3 class="text-2xl sm:text-3xl md:text-5xl">
                            {benefit.name}
                        </h3>
                        <p>{benefit.description}</p>
                    </div>
                </div>
            {/each}
        </div>
        

    </section>
</main>
