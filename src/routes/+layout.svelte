<script>
    import "../app.css";

    let { children } = $props();
</script>

<svelte:head>
    <title>Logan's Portfolio</title>
</svelte:head>

<div class="min-h-screen flex flex-col">
    <div class="mb-4">
        <div class="flex justify-center">
            <div class="flex flex-col md:flex-row md:space-x-40 mt-5 border-b w-3/4 md:w-1/2
        items-center md:justify-center pb-3 border-white/60">
                <div class="hidden md:block">
                    <h1 class="text-xl">Logan's Portfolio</h1>
                </div>
                <div class="flex space-x-4">
                    <a href="/" class="text-lg">Home</a>
                    <a href="/contact" class="text-lg">Contact</a>
                </div>
            </div>
        </div>
        {@render children?.()}
    </div>
    <footer class="mt-auto items-center justify-center flex h-10 w-full">
        <p class="text-center text-white/90">Created with &hearts; by Logan</p>
    </footer>
</div>
