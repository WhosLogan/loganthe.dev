<script>
    let className = "";
    let title = "";

    // noinspection ReservedWordAsName
    export {className as class, title};
</script>

<div class="bg-neutral-800/80 {className} p-3 max-w-96 border border-white/60 rounded">
    <div class="w-1/2 border-b mb-3">
        <h1 class="text-lg font-bold">{title}</h1>
    </div>
    <slot />
</div>