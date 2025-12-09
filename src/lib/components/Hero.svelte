<script lang="ts">
    // Using a placeholder image that resembles the metallic structure in the screenshot
    const bgImage = "https://images.unsplash.com/photo-1541873676-a18131494184?q=80&w=2818&auto=format&fit=crop";
</script>

<section class="relative h-screen w-full overflow-hidden bg-black text-white">
    <!-- Background Image -->
    <div class="absolute inset-0">
        <img src={bgImage} alt="Space Station Interior" class="w-full h-full object-cover opacity-80" />
        <!-- Gradient Overlay -->
        <div class="absolute inset-0 bg-gradient-to-t from-black/60 via-transparent to-black/30"></div>
    </div>

    <!-- Content -->
    <div class="relative z-10 h-full flex flex-col justify-end px-6 pb-20 md:px-12 md:pb-32 max-w-[1400px] mx-auto">
        <h1 class="text-5xl md:text-7xl lg:text-8xl font-semibold leading-[0.95] tracking-tight max-w-4xl mb-12">
            Building<br />
            next-generation<br />
            space stations
        </h1>

        <!-- Video Controls -->
        <div class="flex items-center gap-4">
            <button class="w-10 h-10 border border-white/30 flex items-center justify-center hover:bg-white/10 transition-colors" aria-label="Pause video">
                <div class="flex gap-1">
                    <div class="w-0.5 h-3 bg-white"></div>
                    <div class="w-0.5 h-3 bg-white"></div>
                </div>
            </button>
            <a href="#" class="flex items-center gap-2 text-sm font-medium hover:opacity-70 transition-opacity group">
                <span class="text-xs group-hover:translate-x-1 transition-transform duration-300">›</span>
                Watch full video
            </a>
        </div>
    </div>
</section>
