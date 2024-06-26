<script lang="ts">
    import { Button } from "$lib/components/ui/button/index.js";
    import * as Card from "$lib/components/ui/card/index.js";
    import { Input } from "$lib/components/ui/input/index.js";
    import { Label } from "$lib/components/ui/label/index.js";
    import { site_name } from "$lib/config";
  </script>
  

<svelte:head>
    <title>
        Signup - {site_name}
    </title>
</svelte:head>

<div class="max-w-5xl mx-auto p-4 flex justify-center">
  <Card.Root class="w-full max-w-sm mt-10">
    <Card.Header>
      <Card.Title class="text-2xl">Create an account</Card.Title>
      <Card.Description>Enter your email below to create an account.</Card.Description>
    </Card.Header>
    <Card.Content class="grid gap-4">
      <div class="grid gap-2">
        <Label for="name">Name</Label>
        <Input id="name" type="name" placeholder="Full Name" required />
      </div>
      <div class="grid gap-2">
        <Label for="email">Email</Label>
        <Input id="email" type="email" placeholder="Email Address" required />
      </div>
      <div class="grid gap-2">
        <Label for="password">Password</Label>
        <Input id="password" type="password" placeholder="Password" required />
      </div>
    </Card.Content>
    <Card.Footer>
      <Button class="w-full">Signup</Button>
    </Card.Footer>
  </Card.Root>
</div>
  