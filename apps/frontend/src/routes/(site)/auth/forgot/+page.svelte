<script lang="ts">
    import { Button } from "$lib/components/ui/button/index.js";
    import * as Card from "$lib/components/ui/card/index.js";
    import { Input } from "$lib/components/ui/input/index.js";
    import { Label } from "$lib/components/ui/label/index.js";
    import { site_name } from "$lib/config";
  </script>
  

<svelte:head>
    <title>
        Forgot Password - {site_name}
    </title>
</svelte:head>

<div class="max-w-5xl mx-auto p-4 flex justify-center">
  <Card.Root class="w-full max-w-sm mt-10">
    <Card.Header>
      <Card.Title class="text-2xl">Forgot Password?</Card.Title>
      <Card.Description>Enter your email below to reset your password</Card.Description>
    </Card.Header>
    <Card.Content class="grid gap-4">
      <div class="grid gap-2">
        <Label for="email">Email</Label>
        <Input id="email" type="email" placeholder="Email Address" required />
      </div>

    </Card.Content>
    <Card.Footer class="block">
      <Button class="w-full">Send Instructions</Button>
      <Button class="w-full mt-2" variant="link" href="/auth/login">Login</Button>
    </Card.Footer>
  </Card.Root>
</div>
  