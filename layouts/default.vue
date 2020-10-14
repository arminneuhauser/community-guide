<template>
  <div>
    <site-header/>
    <main class="main" role="main">
      <Nuxt />
      <aside class="sitebar"></aside>
    </main>
    <site-footer/>
  </div>
</template>

<style lang="scss">
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

  @include breakpoint(l) {
    display: grid;
    grid-template-columns: auto 300px;
    padding-top: 86px;
  }

  .sitebar {
    width: 100%;
    height: 100%;
    background: rgba(0,0,0,0.1);
  }
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
  border: none;
  color: var(--on-cta);
  text-decoration: none;
  padding: 10px 35px;
  text-align: center;
  font-weight: bold;
  display: inline-flex;
}

button {
  cursor: pointer;
}

input, textarea {
  font-family: inherit;
  color: currentColor;
  border: 1px solid var(--border-color);
  padding: 5px 10px;
}

.story {
  padding: var(--site-core-padding);

  article {
    position: relative;
    margin: 20px 0;

    > div {
      > * {
        max-width: 615px;
        margin: 0 auto;
      }
    }
  }

  header {
    h2 {
      font-family: $fs-condensed;
      font-size: 1.6rem;
      font-weight: normal;
      text-transform: uppercase;
      margin: 0 0 6px;
    }
    h1 {
      font-family: $fs-condensed;
      font-size: 3.2rem;
      line-height: 1;
      margin: 0 0 8px;
    }
    p {
      font-size: 1.8rem;
      margin: 0 0 8px;
    }
  }

  .body {
    font-size: 1.7rem;
    line-height: 2.6rem;
  }

  figure {
    margin: 20px 0;

    p {
      font-size: 1.5rem;
      line-height: 2.1rem;
      margin: 15px 0 0;
    }
    footer {
      font-size: 1.2rem;
      line-height: 1.4rem;
      margin: 6px 0 0;
      opacity: 0.3;
    }
  }
}
</style>
