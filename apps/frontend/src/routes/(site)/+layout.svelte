<script lang="ts">
	import { Button } from '$lib/components/ui/button';
    import { site_name, site_logo_dark, site_title } from "$lib/config";

</script>

<svelte:head>
    <title>
        {site_name} - {site_title}
    </title>
</svelte:head>


<div class="relative z-20 pt-[60px] md:h-screen md:max-h-[950px] md:pt-0">

    <!-- Header -->
    <div class="max-w-5xl mx-auto sticky top-0">

        
        <div class="p-4">
            <div class=" flex items-center justify-between py-2 px-5 rounded-2xl border dark:border-muted/80 backdrop-blur-3xl shadow-md">
                <a href="/" class="inline-flex items-center gap-2 select-none">
                        <img class="size-5" src={site_logo_dark} alt={site_name}>
                        <p class="text-sm font-inter-500">{site_name}</p>
                </a>
                <div class="text-sm space-x-2 flex items-center">


                    <Button href="/" variant="link" size="sm">Pricing</Button>
                    <Button href="/" variant="link" size="sm">Features</Button>
                    <Button href="/auth/login" variant="outline" size="sm">Login</Button>
                    <Button href="/auth/signup" variant="default" size="sm">Signup</Button>
                </div>
            </div>
        </div>


    </div>
    <!-- Header -->

    <img alt="Light ray background" fetchpriority="high" width="1000" height="1000" decoding="async" data-nimg="1" class="pointer-events-none absolute -top-20 left-0 right-0 z-0 mx-auto hidden h-full w-full select-none md:block" style="color: transparent;" srcset="/_next/image?url=%2Fstatic%2Flanding-page%2Fbghero.png&amp;w=1080&amp;q=75 1x, https://resend.com/_next/image?url=%2Fstatic%2Flanding-page%2Fbghero.png&w=2048&q=75 2x" src="https://resend.com/_next/image?url=%2Fstatic%2Flanding-page%2Fbghero.png&w=2048&q=75">


<slot />

</div>