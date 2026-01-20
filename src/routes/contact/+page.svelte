<script>
    import ContentBox from "$lib/ContentBox.svelte";
    import { fade } from 'svelte/transition';
</script>

<svelte:head>
    <meta name="description" content="Get in contact with Logan for development work or general purpose communication." />
</svelte:head>

<div class="flex flex-col items-center mt-8" in:fade>
    <h1 class="mb-8 text-xl font-bold">Contact Me</h1>
    <ContentBox title="Contact Info">
        <p>You may contact me via the following methods</p>
        <ul class="list-disc ml-4">
            <li>&#x2709; <a href="mailto:logan@loganthe.dev">logan@loganthe.dev</a></li>
            <li>&#x2709; <a href="mailto:logan@reallyprivate.email">logan@reallyprivate.email</a></li>
        </ul>
    </ContentBox>
</div>