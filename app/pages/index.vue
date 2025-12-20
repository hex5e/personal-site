<template>
  <main class="landing">
    <div class="chevrons" aria-hidden="true">
      <svg
        class="chevronsSvg"
        viewBox="0 0 220 760"
        role="presentation"
        focusable="false"
      >
        <g transform="translate(0, 20)">
          <path
            class="chevronOutline"
            d="M 20 0 L 110 70 L 200 0 L 178 0 L 110 52 L 42 0 Z"
          />

          <g transform="translate(0, 95)">
            <path
              class="chevronFill"
              d="M 20 0 L 110 70 L 200 0 L 178 0 L 110 52 L 42 0 Z"
            />
          </g>
          <g transform="translate(0, 190)">
            <path
              class="chevronFill"
              d="M 20 0 L 110 70 L 200 0 L 178 0 L 110 52 L 42 0 Z"
            />
          </g>
          <g transform="translate(0, 285)">
            <path
              class="chevronFill"
              d="M 20 0 L 110 70 L 200 0 L 178 0 L 110 52 L 42 0 Z"
            />
          </g>
          <g transform="translate(0, 380)">
            <path
              class="chevronFill"
              d="M 20 0 L 110 70 L 200 0 L 178 0 L 110 52 L 42 0 Z"
            />
          </g>
          <g transform="translate(0, 475)">
            <path
              class="chevronFill"
              d="M 20 0 L 110 70 L 200 0 L 178 0 L 110 52 L 42 0 Z"
            />
          </g>
          <g transform="translate(0, 570)">
            <path
              class="chevronFill"
              d="M 20 0 L 110 70 L 200 0 L 178 0 L 110 52 L 42 0 Z"
            />
          </g>
          <g transform="translate(0, 665)">
            <path
              class="chevronOutline"
              d="M 20 0 L 110 70 L 200 0 L 178 0 L 110 52 L 42 0 Z"
            />
          </g>
        </g>
      </svg>
    </div>

    <div class="content">
      <h1 class="title">
        <NuxtLink class="titleLink" to="/">hex5e</NuxtLink>
      </h1>

      <nav class="nav" aria-label="Primary">
        <a
          class="navLink"
          href="https://discord.com/users/hex5e"
          target="_blank"
          rel="noopener noreferrer"
        >
          discord
        </a>
        <a
          class="navLink"
          href="https://github.com/hex5e"
          target="_blank"
          rel="noopener noreferrer"
        >
          github
        </a>
        <NuxtLink class="navLink" to="/blog">blog</NuxtLink>
      </nav>
    </div>
  </main>
</template>

<style scoped>
.landing {
  --bg: #6e6e6e;
  --fg: #f4f4f4;

  min-height: 100vh;
  background: var(--bg);
  color: var(--fg);

  display: grid;
  grid-template-columns: 320px 1fr;
  align-items: start;
}

.chevrons {
  padding: 40px 0 40px 40px;
}

.chevronsSvg {
  width: 220px;
  height: auto;
  display: block;
  transform: rotate(180deg);
  transform-origin: 50% 50%;
}

.chevronOutline {
  fill: none;
  stroke: var(--fg);
  stroke-width: 6;
  stroke-linejoin: bevel;
}

.chevronFill {
  fill: var(--fg);
}

.content {
  padding: 70px 40px;
}

.title {
  margin: 0;
  font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas,
    "Liberation Mono", "Courier New", monospace;
  font-weight: 300;
  font-size: 96px;
  line-height: 1;
}

.titleLink {
  color: inherit;
  text-decoration-line: underline;
  text-decoration-thickness: 6px;
  text-underline-offset: 12px;
}

.nav {
  margin-top: 80px;
  display: flex;
  flex-direction: column;
  gap: 18px;
}

.navLink {
  font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas,
    "Liberation Mono", "Courier New", monospace;
  font-weight: 300;
  font-size: 72px;
  line-height: 1.05;
  color: inherit;
  text-decoration: none;
}

@media (max-width: 900px) {
  .landing {
    grid-template-columns: 1fr;
  }

  .chevrons {
    padding: 28px 24px 0 24px;
  }

  .chevronsSvg {
    width: 180px;
  }

  .content {
    padding: 24px;
  }

  .title {
    font-size: 72px;
  }

  .nav {
    margin-top: 40px;
  }

  .navLink {
    font-size: 56px;
  }
}
</style>
