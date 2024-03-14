<script>
    export let title;
    export let content;
    export let linkTitle;
    export let linkPath;
    export let imageSrc;
</script>
<section class="hero py-[2.5rem] md:py-[5rem]">
    <div class="relative max-w-[58.5rem] mx-auto flex flex-col justify-center items-center px-2 md:px-0 gap-y-3 md:gap-y-[3rem] lg:gap-y-[6.5rem]">
        <div class="flex flex-col justify-center items-center max-w-[49.125rem] mx-auto">
            {#if title}
            <h1 class="text-[3rem] leading-[3.75rem] lg:text-[4.5rem] lg:leading-[5rem] text-center font-bold text-slate-700">{title}</h1>
            {/if}
            {#if content}
            <p class="text-[1.5rem] text-center mt-[0.5rem] text-slate-600">{content}</p> 
            {/if}
            {#if linkPath}
            <a href={linkPath} class="inline-flex items-center justify-center text-center px-[3.5rem] py-[0.75rem] rounded-full bg-[#0E7490] text-white mt-[2rem]">{linkTitle}</a>
            {/if}
        </div>
        {#if imageSrc}
        <div class="relative w-full block pb-[72%]">
            <img src={imageSrc} alt="" class="absolute top-0 left-0 h-full w-full object-cover"/>
        </div>
        {/if}
    </div>
</section>