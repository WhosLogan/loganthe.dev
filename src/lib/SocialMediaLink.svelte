<script>
    export let title;
    export let link;
    export let image;
</script>

<a href="{link}" target="_blank" rel="noopener noreferrer" class="hover:bg-neutral-700/70 w-full flex items-center space-x-3 px-3 py-2 rounded">
    <img class="max-w-8" src={image} alt="{title} image" />
    <p class="font-semibold">{title}</p>
</a>