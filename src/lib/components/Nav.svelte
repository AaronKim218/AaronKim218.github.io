<script>
  let ROUTES = [
    { name: 'Home', path: '/' },
    { name: 'Projects', path: '/projects' },
    { name: 'Resume', path: '/resume' },
    { name: 'Contact', path: '/contact' }
  ];
</script>

<nav>
  <ul>
    {#each ROUTES as { name, path }}
      <li><a href={path}>{name}</a></li>
    {/each}
  </ul>
</nav>

<style>
  nav {
    display: flex;
    justify-content: center;
    background-color: var(--primary-color);
    padding: 1rem;
  }

  ul {
    display: flex;
  }

  li {
    margin: 0 2rem;
  }

  a {
    font-size: 1.5rem;
    text-decoration: none;
    color: var(--background-color);
  }
</style>
