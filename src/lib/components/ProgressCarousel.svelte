<script lang="ts">
    const carouselImage = "https://images.unsplash.com/photo-1446776811953-b23d57bd21aa?q=80&w=2072&auto=format&fit=crop";
    const nextImage = "https://images.unsplash.com/photo-1516849841032-87cbac4d88f7?q=80&w=2070&auto=format&fit=crop";
</script>

<section class="bg-white py-24 px-6 md:px-12 overflow-hidden">
    <div class="max-w-[1400px] mx-auto">
        <h2 class="text-4xl md:text-5xl lg:text-6xl font-semibold leading-[1.05] tracking-tight mb-16 text-black">
            Haven-1 hardware development<br />
            progress
        </h2>

        <!-- Carousel Container -->
        <div class="relative w-full flex gap-6 overflow-hidden">
            <!-- Slide 1 -->
            <div class="relative w-full md:w-[85%] shrink-0 aspect-[16/9] bg-gray-900 group">
                <img src={carouselImage} alt="Hardware development" class="w-full h-full object-cover opacity-80 group-hover:opacity-100 transition-opacity duration-500" />
                
                <!-- Overlay Card -->
                <div class="absolute bottom-0 left-0 p-8 md:p-12 w-full md:w-1/2 bg-gradient-to-t from-black/80 via-black/40 to-transparent md:bg-none">
                    <div class="flex items-center gap-2 mb-4">
                        <div class="w-2 h-2 bg-white"></div>
                        <span class="text-[10px] font-mono font-bold tracking-wider text-white uppercase">Mission Success</span>
                    </div>
                    
                    <div class="text-[10px] font-mono text-gray-400 mb-4 uppercase tracking-wider">November 2, 2025</div>
                    
                    <p class="text-white text-lg leading-relaxed mb-8">
                        Haven Demo achieved mission success after deploying from the Bandwagon-4 rideshare mission. The spacecraft captured 4K video of its solar array deployment and is now power positive.
                    </p>
                    
                    <a href="#" class="flex items-center gap-2 text-sm font-medium text-white hover:opacity-70 transition-opacity group/link">
                        <span class="text-xs group-hover/link:translate-x-1 transition-transform duration-300">›</span>
                        Watch the video
                    </a>
                </div>
            </div>

            <!-- Slide 2 (Partial) -->
            <div class="relative w-full md:w-[85%] shrink-0 aspect-[16/9] bg-gray-800 hidden md:block opacity-50">
                <img src={nextImage} alt="Next slide" class="w-full h-full object-cover grayscale" />
                <div class="absolute bottom-12 left-12">
                    <div class="flex items-center gap-2 mb-4">
                        <div class="w-2 h-2 bg-white"></div>
                        <span class="text-[10px] font-mono font-bold tracking-wider text-white uppercase">The Next Phase</span>
                    </div>
                    <div class="text-[10px] font-mono text-gray-400 mb-4 uppercase tracking-wider">October 29, 2025</div>
                    <p class="text-white text-lg leading-relaxed mb-8 max-w-md truncate">
                        The flight primary structure has arrived at Vast headquarters...
                    </p>
                     <a href="#" class="flex items-center gap-2 text-sm font-medium text-white hover:opacity-70 transition-opacity group/link">
                        <span class="text-xs group-hover/link:translate-x-1 transition-transform duration-300">›</span>
                        Watch the video
                    </a>
                </div>
            </div>
        </div>

        <!-- Controls -->
        <div class="flex flex-col md:flex-row items-end md:items-center justify-between mt-8 pt-8 border-t border-gray-200 gap-6">
            <div class="text-[10px] font-mono text-gray-500 uppercase tracking-wider max-w-xs leading-relaxed">
                See the manufacturing and testing process of Haven-1, the world's first commercial space station.
            </div>

            <!-- Progress Bar -->
            <div class="flex-1 w-full flex items-center justify-center px-4 md:px-12">
                <div class="flex gap-1">
                    <div class="w-1 h-4 bg-[#FF4D00]"></div>
                    {#each Array(20) as _}
                        <div class="w-px h-2 bg-gray-300"></div>
                    {/each}
                </div>
            </div>

            <!-- Arrows -->
            <div class="flex gap-2">
                <button class="w-10 h-10 bg-[#B0A89E] hover:bg-[#9e968d] transition-colors flex items-center justify-center text-white disabled:opacity-50">
                    <span class="text-xl">‹</span>
                </button>
                <button class="w-10 h-10 bg-[#B0A89E] hover:bg-[#9e968d] transition-colors flex items-center justify-center text-white">
                    <span class="text-xl">›</span>
                </button>
            </div>
        </div>
    </div>
</section>
