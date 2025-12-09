<script lang="ts">
    const demoImage = "https://images.unsplash.com/photo-1451187580459-43490279c0fa?q=80&w=2072&auto=format&fit=crop";
</script>

<section class="bg-white py-24 px-6 md:px-12 text-black">
    <div class="max-w-[1400px] mx-auto">
        <!-- Text Header -->
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 mb-16">
            <h2 class="text-4xl md:text-5xl lg:text-6xl font-semibold leading-[1.05] tracking-tight">
                Haven Demo:<br />
                In-space testbed for Haven-1 space station technologies
            </h2>
            <div class="flex flex-col justify-between">
                <p class="text-lg md:text-xl leading-relaxed text-gray-800 max-w-xl">
                    In November 2025, Haven Demo achieved mission success after deploying from SpaceX’s Bandwagon-4 flight. The spacecraft captured 4K video of its solar array deployment and is now power-positive.
                </p>
                <a href="#" class="inline-flex items-center gap-2 mt-8 text-sm font-medium hover:opacity-70 transition-opacity group">
                    <span class="text-xs group-hover:translate-x-1 transition-transform duration-300">›</span>
                    Learn more
                </a>
            </div>
        </div>

        <!-- Media Content -->
        <div class="relative w-full aspect-video bg-gray-900 overflow-hidden group">
            <img src={demoImage} alt="Earth from space with spacecraft components" class="w-full h-full object-cover" />
            
            <!-- Video Controls Overlay -->
            <div class="absolute bottom-8 left-8 flex items-center gap-4 z-10">
                <button class="w-10 h-10 bg-black/50 backdrop-blur-sm border border-white/20 flex items-center justify-center hover:bg-black/70 transition-colors text-white" aria-label="Pause video">
                    <div class="flex gap-1">
                        <div class="w-0.5 h-3 bg-white"></div>
                        <div class="w-0.5 h-3 bg-white"></div>
                    </div>
                </button>
                <a href="#" class="flex items-center gap-2 text-sm font-medium text-white hover:opacity-70 transition-opacity group">
                    <span class="text-xs group-hover:translate-x-1 transition-transform duration-300">›</span>
                    Watch full video
                </a>
            </div>
        </div>
        <div class="flex justify-end mt-2">
             <span class="text-[10px] font-mono tracking-wider text-gray-500 uppercase">Launch video courtesy of SpaceX</span>
        </div>
    </div>
</section>
