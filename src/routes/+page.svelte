<script>
    import ContentBox from "$lib/ContentBox.svelte";
    import SocialMediaLink from "$lib/SocialMediaLink.svelte";
    import ProjectLink from "$lib/ProjectLink.svelte";
    import {fade} from "svelte/transition";
</script>

<div class="flex flex-col items-center mt-8" in:fade>
    <h1 class="mb-8 text-xl font-bold">Welcome to my portfolio</h1>
    <div class="grid grid-cols-1 md:grid-cols-2 gap-10 mx-3">
        <ContentBox title="About Me">
            <p>I'm Logan, a highly motivated software developer with years in the industry.
                I have worked for and owned many startups in the past and I have led
                companies and projects to success numerous times. I strive to create
                ground-breaking projects while fostering a fun and inclusive work environment.</p>
        </ContentBox>
        <ContentBox title="Social Media" class="">
            <div class="mt-3 space-y-1">
                <SocialMediaLink title="Github" link="https://github.com/WhosLogan" image="/assets/github.svg" />
                <SocialMediaLink title="Linkedin" link="https://www.linkedin.com/in/loganmonty04/" image="/assets/linkedin.png" />
            </div>
        </ContentBox>
        <ContentBox title="Projects" class="md:max-w-none md:col-span-2">
            <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                <ProjectLink title="Cloak" description="An easy to learn from .NET obfuscator"
                             link="https://github.com/WhosLogan/Cloak" lang="csharp" />
                <ProjectLink title="loganthe.dev" description="My personal portfolio (this exact website!)"
                             link="https://github.com/WhosLogan/loganthe.dev" lang="ts" />
                <ProjectLink title="OneUpload" description="An easy way to receive uploaded files from users"
                             link="https://github.com/WhosLogan/OneUpload" lang="ts" />
                <ProjectLink title="ExifStripper" description="An easy way to strip exif data from images"
                             link="https://github.com/WhosLogan/ExifStripper" lang="csharp" />
            </div>
        </ContentBox>
    </div>
</div>