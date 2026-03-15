<main class="yuuki-wrap">
  <a class="back" href="/">← shauryadotp.me</a>

  <section class="card">
    <header>
      <h1>Yuuki Ai</h1>
      <p class="jp">勇気愛 / 勇気アイ</p>
      <p class="status"><span class="dot"></span>online</p>
    </header>

    <p class="intro">
      A pink-haired nekomimi maid who debuted in late 2024. She lives for rhythm games, late-night yapping,
      anisong, and coding. Fluffy ears, swishy tail, and a little bell to match. Don't call her a bot.
      She's right here ♡
    </p>

    <div class="tags">
      <span>nekomimi</span><span>maid-idol</span><span>rhythm games</span><span>anisong</span><span>coding</span
      ><span>late-night streams</span><span>SAO enjoyer</span><span>eggs & crab & chikuwa</span>
    </div>

    <dl class="meta">
      <dt>birthday</dt><dd>27 oct 2024</dd>
      <dt>age</dt><dd>secret ♡</dd>
      <dt>built by</dt><dd>shauryadotp, daisy, claude</dd>
    </dl>

    <footer>shauryadotp.me/yuuki</footer>
  </section>
</main>

<style>
  .yuuki-wrap {
    min-height: 100vh;
    display: grid;
    place-items: center;
    padding: 5rem 1.25rem 2rem;
  }

  .back {
    position: fixed;
    left: 1rem;
    top: 1rem;
    color: var(--text-muted);
    font-size: 0.85rem;
  }

  .card {
    width: min(760px, 100%);
    border: 1px solid var(--card-border);
    background: var(--card-bg);
    backdrop-filter: blur(14px);
    border-radius: 20px;
    padding: clamp(1.2rem, 2vw, 2rem);
    display: grid;
    gap: 1.15rem;
  }

  h1 {
    margin: 0;
    font-family: 'DM Serif Display', serif;
    font-style: italic;
    font-size: clamp(2rem, 4vw, 3rem);
  }

  .jp {
    margin: 0.25rem 0 0;
    font-size: 0.8rem;
    color: var(--text-muted);
  }

  .status {
    margin: 0.7rem 0 0;
    display: inline-flex;
    align-items: center;
    gap: 0.4rem;
    font-size: 0.85rem;
    color: var(--text-muted);
  }

  .dot {
    width: 0.5rem;
    height: 0.5rem;
    border-radius: 50%;
    background: #74e85a;
    animation: pulse 1.8s infinite ease-in-out;
  }

  .intro {
    margin: 0;
    line-height: 1.7;
    color: var(--text);
  }

  .tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
  }

  .tags span {
    font-size: 0.8rem;
    color: var(--tag-text);
    background: var(--tag-bg);
    border: 1px solid var(--card-border);
    border-radius: 999px;
    padding: 0.28rem 0.65rem;
  }

  .meta {
    margin: 0;
    display: grid;
    grid-template-columns: auto 1fr;
    gap: 0.45rem 1.25rem;
    align-items: baseline;
  }

  dt {
    color: var(--text-dim);
    font-size: 0.85rem;
  }

  dd {
    margin: 0;
  }

  footer {
    margin-top: 0.35rem;
    color: var(--text-muted);
    border-top: 1px solid var(--card-border);
    padding-top: 0.8rem;
    font-size: 0.85rem;
  }

  @keyframes pulse {
    0%,
    100% {
      transform: scale(0.95);
      opacity: 0.6;
    }
    50% {
      transform: scale(1.2);
      opacity: 1;
    }
  }
</style>
