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
        <a href="/" class="flex items-center gap-3">
            <svg width="38" height="37" viewBox="0 0 95 92" fill="none" xmlns="http://www.w3.org/2000/svg" class="{isScrolled ? 'text-black' : 'text-white'}">
                <path d="M22.0497 45.9167C22.0497 32.5699 32.8409 21.75 46.1523 21.75C59.4639 21.75 70.2549 32.5699 70.2549 45.9167H91.9472C91.9472 20.5576 71.4441 0 46.1523 0C20.8605 0 0.357424 20.5576 0.357422 45.9167C0.35742 71.2757 20.8605 91.8333 46.1523 91.8333V70.0833C32.8409 70.0833 22.0497 59.2637 22.0497 45.9167Z" fill="currentColor"/>
                <path opacity="0.5" d="M70.2548 45.9166C70.2548 59.2634 81.046 70.0833 94.3574 70.0833V91.8333C69.0656 91.8333 48.5625 71.2757 48.5625 45.9166H70.2548Z" fill="currentColor"/>
            </svg>
            <span class="text-xl font-bold tracking-tight">DiligenceSquared</span>
        </a>
    </div>

    <!-- Center Links -->
    <div class="hidden md:flex items-center gap-8 text-sm font-medium tracking-wide">
        <a href="#platform" class="hover:opacity-70 transition-opacity">Platform</a>
        <a href="#how-it-works" class="hover:opacity-70 transition-opacity">How It Works</a>
        <a href="#case-studies" class="hover:opacity-70 transition-opacity">Case Studies</a>
        <a href="#about" class="hover:opacity-70 transition-opacity">About</a>
    </div>

    <!-- Right Actions -->
    <div class="flex items-center gap-6">
        <a href="#contact" class="text-sm font-medium hover:opacity-70 transition-opacity hidden sm:block">Contact</a>
        <a href="#demo" class="bg-white text-black px-5 py-2.5 text-xs font-semibold uppercase tracking-wide hover:bg-gray-200 transition-colors {isScrolled ? '!bg-black !text-white hover:!bg-gray-800' : ''}">
            Schedule Demo
        </a>
    </div>
</nav>
