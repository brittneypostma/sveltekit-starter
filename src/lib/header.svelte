<script>
  import { page } from '$app/stores'
</script>

<header>
  <div class="left">
    <img src="svelte-logo.svg" alt="svelte logo" />
  </div>
  <nav>
    <ul>
      <li class:active={$page.path === '/'}>
        <a href="/">Home</a>
      </li>
      <li class:active={$page.path === '/about'}>
        <a href="/about">About</a>
      </li>
      <li class:active={$page.path === '/blog'}>
        <a href="/blog">Blog</a>
      </li>
    </ul>
  </nav>
  <div class="right" />
</header>

<style>
  .left img {
    margin-left: 1rem;
    width: 2rem;
    height: 2rem;
    object-fit: contain;
  }
  header {
    height: var(--header-height);
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  nav {
    background: var(--color-primary);
    box-shadow: var(--shadow-lg);
    padding: var(--md) var(--xl);
    border-radius: 0 0 var(--xl) var(--xl);
  }
  ul {
    display: flex;
    justify-content: space-between;
    gap: var(--base);
  }
  a {
    text-shadow: var(--shadow-text);
  }
  .active {
    border-bottom: 2px solid var(--color-accent);
  }
</style>
