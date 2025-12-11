<script lang="ts">
    const demoImage = "/generated/image-business-professional-conducting-a-video-1765456503425-1.webp";
</script>

<section id="platform" class="bg-white py-24 px-6 md:px-12 text-black">
    <div class="max-w-[1400px] mx-auto">
        <!-- Text Header -->
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 mb-16">
            <h2 class="text-4xl md:text-5xl lg:text-6xl font-semibold leading-[1.05] tracking-tight">
                AI-Moderated Interviews:<br />
                Expert insights at scale
            </h2>
            <div class="flex flex-col justify-between">
                <p class="text-lg md:text-xl leading-relaxed text-gray-800 max-w-xl">
                    Our AI voice agents conduct in-depth interviews in multiple languages, delivering investor-grade insights in days instead of weeks. Every finding traces back to actual conversations, providing analytical depth beyond traditional consulting.
                </p>
                <a href="#how-it-works" class="inline-flex items-center gap-2 mt-8 text-sm font-medium hover:opacity-70 transition-opacity group">
                    <span class="text-xs group-hover:translate-x-1 transition-transform duration-300">›</span>
                    Learn more
                </a>
            </div>
        </div>

        <!-- Media Content -->
        <div class="relative w-full aspect-video bg-gray-900 overflow-hidden group">
            <img src={demoImage} alt="Professional conducting AI-moderated interview" class="w-full h-full object-cover" />
            
            <!-- Info Overlay -->
            <div class="absolute bottom-8 left-8 right-8 z-10">
                <div class="bg-black/70 backdrop-blur-sm border border-white/20 p-6 max-w-md">
                    <h3 class="text-white font-semibold text-lg mb-2">Multilingual Support</h3>
                    <p class="text-gray-300 text-sm">Conduct interviews across 5+ countries in local languages, all quality-assured by top-tier consultants.</p>
                </div>
            </div>
        </div>
        <div class="flex justify-end mt-2">
             <span class="text-[10px] font-mono tracking-wider text-gray-500 uppercase">Platform interface</span>
        </div>
    </div>
</section>
