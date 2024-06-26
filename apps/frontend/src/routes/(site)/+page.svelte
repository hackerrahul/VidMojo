<script lang="ts">

    import { Button } from "$lib/components/ui/button";
    import { site_name, site_title } from "$lib/config";

</script>

<svelte:head>
    <title>
        {site_name} - {site_title}
    </title>
</svelte:head>

<div class="max-w-5xl mx-auto p-4">
   
    <div class="mt-10 text-center">
        <p class="text-8xl font-inter-500 bg-gradient-to-bl text-transparent bg-clip-text from-foreground via-foreground/80 to-background">
            AI Powered Video Creator
        </p>
        
        <Button class="mt-6 rounded-xl" variant="default" size="lg">Get Started</Button>
    </div>

</div>