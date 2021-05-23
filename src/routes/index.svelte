<script context="module">
  export const prerender = true
</script>

<script>
  import Counter from '$lib/counter.svelte'
</script>

<section>
  <h1>Welcome!</h1>
  <h2>Let's learn Svelte</h2>
  <Counter />
</section>

<style>
  section {
    min-height: calc(100vh - var(--header-height));
    display: grid;
    place-items: center;
    place-content: center;
  }
</style>
