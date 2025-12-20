<template>
  <main class="blog">
    <div class="content">
      <h1 class="title">blog</h1>
      <ul class="list">
        <li><NuxtLink class="link" to="/blog/yet-another-anki-appreciation-post">Yet Another Anki Appreciation Post</NuxtLink></li>
      </ul>
    </div>
  </main>
</template>

<style scoped>
.blog {
  --bg: #6e6e6e;
  --fg: #f4f4f4;

  min-height: 100vh;
  background: var(--bg);
  color: var(--fg);
}

.content {
  padding: 70px 40px;
}

.title {
  margin: 0 0 40px 0;
  font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas,
    "Liberation Mono", "Courier New", monospace;
  font-weight: 300;
  font-size: 72px;
  line-height: 1;
}

.list {
  margin: 0;
  padding: 0;
  list-style: square;
}

.link {
  font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas,
    "Liberation Mono", "Courier New", monospace;
  font-weight: 300;
  font-size: 56px;
  line-height: 1.05;
  color: inherit;
  text-decoration: none;
}

.link:hover {
  text-decoration: underline;
  text-decoration-thickness: 6px;
  text-underline-offset: 10px;
}

@media (max-width: 900px) {
  .content {
    padding: 24px;
  }

  .title {
    font-size: 56px;
  }

  .link {
    font-size: 44px;
  }
}
</style>
