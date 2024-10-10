<script>
    export let title;
    export let description;
    export let link;
    export let lang;
</script>

<a href="{link}" target="_blank" rel="noopener noreferrer">
    <div class="p-5 bg-neutral-800 hover:bg-neutral-700/60 h-40 flex flex-col rounded">
        <p class="font-semibold text-lg">{title}</p>
        <p class="mt-2">{description}</p>
        <div class="mt-auto flex space-x-4 items-center">
            <img class="w-10" src="/assets/github.svg" alt="Github Logo" />
            <img class="w-10" src="/assets/lang-{lang}.svg" alt="{lang} Logo" />
        </div>
    </div>
</a>