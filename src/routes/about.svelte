<script context="module">
  import { browser, dev } from '$app/env'
  export const hydrate = dev
  export const router = browser
  export const prerender = true
</script>

<svelte:head>
  <title>About</title>
</svelte:head>
<section>
  <h1>About</h1>
  <p>This is the about page.</p>
</section>
