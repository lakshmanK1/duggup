<script>
    import Founder from "./Founder.svelte";
    import Card from "./Card.svelte";

    const firstSection = [
        {info:'No amount of technology can convert a bad story into good story.', image:"images/1stSectionOne.png"},
        {info:"Most people don't have original ideas. Here is how Sam Altman pushes himself to have original ideas which makes him creative person.", image:"images/1stSectionTwo.png"}
    ]

    const secondSection = [
        {info:`Startup Lesson Iam reflecting. Don't build for the "average person"`, image:"images/2ndSectionOne.png"},
        {info:"Your biggest regrets at 80 will be acts of omission", image:"images/2ndSectionTwo.png"}
    ]

    const thirdSection = [
        {info:`Startup Lesson Iam reflecting. Don't build for the "average person"`, image:"images/2ndSectionTwo.png"},
        {info:"Your biggest regrets at 80 will be acts of omission", image:"images/1stSectionOne.png"}
    ]
</script>

<main class="flex flex-col justify-center items-center">
    <section class="sm:w-[800px]">
        <div class="sticky top-0 bg-white py-3 z-10 shadow-xl shadow-white">
            <Founder/>
        </div>
        <div class="timeline">
            <div class="relative">
                <div class="dot"></div>
                <div class="flex justify-center items-center org-year">
                    <p class="text-[#666666] text-end text-xs">Dec 2023</p>
                </div>
                <div class="flex flex-col sm:flex-row justify-between items-center gap-2">
                    {#each firstSection as item}
                        <div class="sm:pl-10">
                            <Card info={item.info} image={item.image}/>
                        </div>                
                    {/each}
                </div>
            </div>

            <div class="relative">
                <div class="dot"></div>
                <div class="flex justify-center items-center org-year">
                    <p class="text-[#666666] text-end text-xs">Dec 2023</p>
                </div>
                <div class="outterdot">
                <div class="innerdot"></div>
                </div>
                <div class="flex flex-col gap-3 org">
                    <div class="flex flex-col">
                        <div class=" flex justify-end items-end">
                            <img src="svg/Logo.svg" class="sm:w-[40px] sm:h-[40px] rounded-full" alt="logo">
                        </div>
                        <p class="text-[#666666] text-end text-xs">San Francisco Bay Area</p>
                        <p class="text-[#666666] text-end text-xs">Joined</p>
                        <p class="text-[#666666] text-end text-xs">Nov 2023</p>
                    </div>
                </div>
                <div class="pl-10">
                    <span class="timeline-date text-[#141618] font-bold">Co-Founder and CEO</span>
                    <h3 class="timeline-title text-[#7A9299]">Full-Time Remote</h3>
                </div>
                <div class="flex flex-col sm:flex-row justify-between items-center gap-2">
                    {#each secondSection as item}
                    <div class="sm:pl-10">
                        <Card info={item.info} image={item.image}/>
                    </div>
                    {/each}
                </div>                
            </div>

            <div class="relative">
                <div class="dot"></div>
                <div class="flex justify-center items-center org-year">
                    <p class="text-[#666666] text-end text-xs">Dec 2023</p>
                </div>
                <div class="outterdot">
                    <div class="innerdot"></div>
                    </div>
                <div class="flex flex-col gap-3 org">
                    <div class="flex flex-col">
                        <div class=" flex justify-end items-end">
                            <img src="svg/betterup.svg" class="sm:w-[40px] sm:h-[40px] rounded-full" alt="logo">
                        </div>
                        <p class="text-[#666666] text-end text-xs">San Francisco Bay Area</p>
                        <p class="text-[#666666] text-end text-xs">Joined</p>
                        <p class="text-[#666666] text-end text-xs">Sep 2022</p>
                    </div>
                </div>
                <div class="pl-10">
                    <span class="timeline-date text-[#141618] font-bold">VP Engineering</span>
                    <h3 class="timeline-title text-[#7A9299]">Full-Time</h3>
                </div>
                <div class="flex flex-col sm:flex-row justify-between items-center gap-2">
                    {#each thirdSection as item}
                    <div class="sm:pl-10">
                        <Card info={item.info} image={item.image}/>
                    </div>
                    {/each}
                </div>                
            </div>
        </div>
</section>
</main>