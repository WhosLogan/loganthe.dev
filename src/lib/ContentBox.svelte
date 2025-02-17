<script>
    let { class: className = "", title = "", children } = $props();
</script>

<div class="bg-neutral-800/40 {className} p-3 max-w-96 border border-white/40 rounded">
    <div class="w-1/2 border-b mb-3">
        <h1 class="text-lg font-bold">{title}</h1>
    </div>
    {@render children?.()}
</div>