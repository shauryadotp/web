<main class="home">
  <h1 data-text="shauryadotp">shauryadotp</h1>
  <p class="sub">builder. tinkerer. 3e8.tech</p>

  <nav>
    <a href="https://github.com/shauryadotp" target="_blank" rel="noreferrer">github</a>
    <a href="https://x.com/shauryadotp" target="_blank" rel="noreferrer">twitter</a>
    <a href="https://instagram.com/shauryadotp" target="_blank" rel="noreferrer">instagram</a>
    <a class="yuuki" href="/yuuki">yuuki →</a>
  </nav>
</main>

<style>
  .home {
    min-height: 100vh;
    display: grid;
    place-content: center;
    gap: 1rem;
    text-align: center;
    padding: 2rem;
  }

  h1 {
    margin: 0;
    font-size: clamp(3rem, 10vw, 7rem);
    font-family: 'DM Serif Display', serif;
    font-style: italic;
    letter-spacing: 0.02em;
    position: relative;
  }

  h1::after {
    content: attr(data-text);
    position: absolute;
    inset: 0;
    color: var(--accent2);
    opacity: 0.25;
    transform: translate(1px, 0);
    animation: glitch 2.8s infinite steps(2, end);
    pointer-events: none;
  }

  .sub {
    margin: 0;
    font-weight: 300;
    color: var(--text-muted);
  }

  nav {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 1.25rem;
  }

  nav a {
    font-weight: 300;
    border-bottom: 1px solid transparent;
    transition: border-color 0.2s ease;
  }

  nav a:hover {
    border-color: currentColor;
  }

  .yuuki {
    color: var(--accent2);
  }

  @keyframes glitch {
    0%,
    100% {
      transform: translate(1px, 0);
    }
    25% {
      transform: translate(-1px, 1px);
    }
    50% {
      transform: translate(0, -1px);
    }
    75% {
      transform: translate(1px, 1px);
    }
  }
</style>
