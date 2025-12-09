<script lang="ts">
    import { onMount } from 'svelte';

    let isScrolled = false;

    onMount(() => {
        const handleScroll = () => {
            isScrolled = window.scrollY > 50;
        };

        window.addEventListener('scroll', handleScroll);
        return () => window.removeEventListener('scroll', handleScroll);
    });
</script>

<nav class="fixed top-0 left-0 w-full z-50 px-6 py-5 flex items-center justify-between transition-all duration-300 {isScrolled ? 'bg-white text-black py-4 shadow-sm' : 'bg-transparent text-white'}">
    <!-- Logo -->
    <div class="flex items-center">
        <a href="/" class="text-2xl font-bold tracking-widest uppercase font-display">Vast</a>
    </div>

    <!-- Center Links -->
    <div class="hidden md:flex items-center gap-8 text-sm font-medium tracking-wide">
        <a href="#" class="hover:opacity-70 transition-opacity">Haven Demo</a>
        <a href="#" class="hover:opacity-70 transition-opacity">Haven-1</a>
        <a href="#" class="hover:opacity-70 transition-opacity">Haven-2</a>
        <a href="#" class="hover:opacity-70 transition-opacity">Roadmap</a>
        <a href="#" class="hover:opacity-70 transition-opacity">About us</a>
    </div>

    <!-- Right Actions -->
    <div class="flex items-center gap-6">
        <a href="#" class="text-sm font-medium hover:opacity-70 transition-opacity hidden sm:block">Shop</a>
        <a href="#" class="bg-white text-black px-5 py-2.5 text-xs font-semibold uppercase tracking-wide hover:bg-gray-200 transition-colors {isScrolled ? '!bg-black !text-white hover:!bg-gray-800' : ''}">
            Create your mission
        </a>
    </div>
</nav>
