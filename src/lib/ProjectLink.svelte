<script>
    let {
        title,
        description,
        link,
        lang
    } = $props();
</script>

<a href="{link}" target="_blank" rel="noopener noreferrer">
    <div class="p-5 bg-neutral-800 hover:bg-neutral-700/60 h-48 flex flex-col rounded max-w-96 space-y-4">
        <p class="font-semibold text-lg">{title}</p>
        <p class="mt-2">{description}</p>
        <div class="mt-auto flex space-x-4 items-center">
            <img class="w-10" src="/assets/github.svg" alt="Github Logo" />
            {#if lang === 'go'}
                <img class="w-14 h-14 scale-x-150 scale-y-150" src="/assets/lang-{lang}.svg" alt="{lang} Logo" />
            {:else}
                <img class="w-10" src="/assets/lang-{lang}.svg" alt="{lang} Logo" />
            {/if}
        </div>
    </div>
</a>