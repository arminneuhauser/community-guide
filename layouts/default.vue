<template>
  <div>
    <site-header/>
    <main class="main" role="main">
      <Nuxt />
    </main>
    <site-footer/>
  </div>
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Roboto+Condensed&family=Roboto:wght@400;700&display=swap');

:root {
  font-size: 62.5%; // 1rem = 10px
}

body {
  font-family: $fs-sans;
  font-size: 1.6rem;
  line-height: 1.4;
  background: var(--background);
  color: var(--on-background);
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

*,
*::before,
*::after {
  box-sizing: border-box;
}

main {
  padding-top: 50px;
}

img {
  max-width: 100%;
  height: auto;
}

figure {
  margin: 0;

  img {
    display: block;
  }
}

.button {
  background: var(--cta);
  color: var(--on-cta);
  text-decoration: none;
  padding: 10px 35px;
  text-align: center;
  font-weight: bold;
}

</style>
