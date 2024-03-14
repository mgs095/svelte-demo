<script>
    export let title;
    export let content;
    export let linkPath;
    export let linkTitle;
    export let imageSrc;
</script>

<section class="hero-left-right py-[1.25rem] md:py-[2.5rem] lg:py-[5rem]">
    <div class="relative max-w-[74.5rem] mx-auto flex flex-col-reverse md:flex-row items-center px-2 lg:px-0 gap-y-[1rem] md:gap-y-0 md:justify-between">
        <div class="flex flex-col justify-start items-start max-w-[30.3125rem] ml-0 mr-auto">
            {#if title}
            <h1 class="text-[3rem] leading-[3.75rem] lg:text-[4.5rem] lg:leading-[5rem] text-left font-bold text-slate-700">{title}</h1>
            {/if}
            {#if content}
            <p class="text-[1.5rem] text-left mt-[1.5rem] md:mt-[0.5rem] text-slate-600">{content}</p> 
            {/if}
            {#if linkPath}
            <a href={linkPath} class="inline-flex items-center justify-center text-center px-[3.5rem] py-[0.75rem] rounded-full bg-[#0E7490] text-white mt-[1.5rem] md:mt-[2rem]">{linkTitle}</a>
            {/if}
        </div>
        {#if imageSrc}
        <div class="relative block pb-[66%] md:pb-[37%] w-full max-h-[14.5rem] md:max-h-0 md:w-[36.4375rem]">
            <img src={imageSrc} alt="" class="absolute top-0 left-0 h-full w-full object-cover rounded-[1rem]"/>
        </div>
        {/if}
    </div>
</section>