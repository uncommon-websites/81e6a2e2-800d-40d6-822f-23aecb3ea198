<script lang="ts">
    const carouselImage = "/generated/image-investment-team-reviewing-market-researc-1765456507960-3.webp";
    const nextImage = "/generated/image-private-equity-professionals-in-a-modern-1765456499944-0.webp";
</script>

<section id="case-studies" class="bg-gray-50 py-24 px-6 md:px-12 overflow-hidden">
    <div class="max-w-[1400px] mx-auto">
        <h2 class="text-4xl md:text-5xl lg:text-6xl font-semibold leading-[1.05] tracking-tight mb-16 text-black">
            Client success stories
        </h2>

        <!-- Carousel Container -->
        <div class="relative w-full flex gap-6 overflow-hidden">
            <!-- Slide 1 - Axcel Case Study -->
            <div class="relative w-full md:w-[85%] shrink-0 aspect-[16/9] bg-gray-900 group">
                <img src={carouselImage} alt="Investment team collaboration" class="w-full h-full object-cover opacity-80 group-hover:opacity-100 transition-opacity duration-500" />
                
                <!-- Overlay Card -->
                <div class="absolute bottom-0 left-0 p-8 md:p-12 w-full md:w-2/3 bg-gradient-to-t from-black/90 via-black/60 to-transparent">
                    <div class="flex items-center gap-2 mb-4">
                        <div class="w-2 h-2 bg-primary-400"></div>
                        <span class="text-[10px] font-mono font-bold tracking-wider text-white uppercase">Nordic PE Portfolio Company</span>
                    </div>
                    
                    <div class="text-[10px] font-mono text-gray-400 mb-4 uppercase tracking-wider">Axcel</div>
                    
                    <p class="text-white text-lg leading-relaxed mb-6">
                        Conducted 60 customer interviews across 5 countries in multiple local languages. The platform's intuitive design and ability to trace every finding back to actual conversations opened up new possibilities for extracting insights.
                    </p>

                    <blockquote class="text-white/90 text-sm italic border-l-2 border-primary-400 pl-4 mb-6">
                        "We were impressed by the depth and quality of customer insights delivered. Being able to trace every finding back to actual customer conversations opened up new possibilities."
                        <footer class="text-xs text-gray-400 mt-2 not-italic">— Oscar Hjort, Associate Director</footer>
                    </blockquote>
                    
                    <a href="#contact" class="flex items-center gap-2 text-sm font-medium text-white hover:opacity-70 transition-opacity group/link">
                        <span class="text-xs group-hover/link:translate-x-1 transition-transform duration-300">›</span>
                        Get started
                    </a>
                </div>
            </div>

            <!-- Slide 2 (Partial) - Mega Cap PE Fund -->
            <div class="relative w-full md:w-[85%] shrink-0 aspect-[16/9] bg-gray-800 hidden md:block opacity-50">
                <img src={nextImage} alt="PE deal team" class="w-full h-full object-cover grayscale" />
                <div class="absolute bottom-12 left-12">
                    <div class="flex items-center gap-2 mb-4">
                        <div class="w-2 h-2 bg-white"></div>
                        <span class="text-[10px] font-mono font-bold tracking-wider text-white uppercase">Mega Cap PE Fund</span>
                    </div>
                    <div class="text-[10px] font-mono text-gray-400 mb-4 uppercase tracking-wider">120 interviews in one week</div>
                    <p class="text-white text-lg leading-relaxed mb-8 max-w-md">
                        Replaced traditional survey-based approaches with AI-moderated interviews, delivering pre-IC insights without large capital commitment...
                    </p>
                     <a href="#contact" class="flex items-center gap-2 text-sm font-medium text-white hover:opacity-70 transition-opacity group/link">
                        <span class="text-xs group-hover/link:translate-x-1 transition-transform duration-300">›</span>
                        Learn more
                    </a>
                </div>
            </div>
        </div>

        <!-- Controls -->
        <div class="flex flex-col md:flex-row items-end md:items-center justify-between mt-8 pt-8 border-t border-gray-300 gap-6">
            <div class="text-[10px] font-mono text-gray-500 uppercase tracking-wider max-w-xs leading-relaxed">
                See how leading PE firms are accelerating their due diligence with DiligenceSquared.
            </div>

            <!-- Progress Bar -->
            <div class="flex-1 w-full flex items-center justify-center px-4 md:px-12">
                <div class="flex gap-1">
                    <div class="w-1 h-4 bg-primary-600"></div>
                    {#each Array(20) as _}
                        <div class="w-px h-2 bg-gray-300"></div>
                    {/each}
                </div>
            </div>

            <!-- Arrows -->
            <div class="flex gap-2">
                <button class="w-10 h-10 bg-gray-900 hover:bg-gray-800 transition-colors flex items-center justify-center text-white disabled:opacity-50">
                    <span class="text-xl">‹</span>
                </button>
                <button class="w-10 h-10 bg-gray-900 hover:bg-gray-800 transition-colors flex items-center justify-center text-white">
                    <span class="text-xl">›</span>
                </button>
            </div>
        </div>
    </div>
</section>
