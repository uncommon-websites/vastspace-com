<script lang="ts">
    import Navbar from "$lib/components/Navbar.svelte";
    import Hero from "$lib/components/Hero.svelte";
    import Statement from "$lib/components/Statement.svelte";
    import HavenDemo from "$lib/components/HavenDemo.svelte";
    import HavenOne from "$lib/components/HavenOne.svelte";
    import ProgressCarousel from "$lib/components/ProgressCarousel.svelte";
</script>

<main class="w-full min-h-screen bg-white">
    <Navbar />
    <Hero />
    <Statement />
    <HavenDemo />
    <HavenOne />
    <ProgressCarousel />
</main>

