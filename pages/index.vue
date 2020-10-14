<template>
  <div class="frontpage">
    <section>
      <article class="teaser">
        <nuxt-link class="teaser-link" to="/story">
          <figure data-type="image">
            <picture>
              <source media="(max-width: 959px)" srcset="//images.derstandard.at/img/2020/10/13/HebeinLudwig.jpg?w=750&amp;s=ed786911">
              <source media="(min-width: 1690px)" srcset="//images.derstandard.at/img/2020/10/13/HebeinLudwig.jpg?w=265&amp;s=409db5da">
              <source media="(min-width: 960px)" srcset="//images.derstandard.at/img/2020/10/13/HebeinLudwig.jpg?w=930&amp;s=f83efd8f">
              <img src="//images.derstandard.at/img/2020/10/13/HebeinLudwig.jpg?w=750&amp;s=ed786911" data-fullscreen-src="//images.derstandard.at/img/2020/10/13/HebeinLudwig.jpg?w=1600&amp;s=a84971dd">
            </picture>
          </figure>
          <header>
            <p class="teaser-kicker">Michael Völker <span>1.163</span></p>
            <h1 class="teaser-title">Grüner Unterwerfungsprozess</h1>
            <p class="teaser-subtitle">Die SPÖ hat es in der Hand, die Grünen aufs Podest oder aus den Angeln zu heben. Die Frage einer Koalition in Wien hat wesentlichen Einfluss auf die Gesamtpartei</p>
          </header>
        </nuxt-link>
      </article>
      <article class="teaser">
        <div>
          <figure data-type="image">
            <picture>
              <source media="(max-width: 959px)" srcset="//images.derstandard.at/img/2020/10/12/bluemel-002.jpg?w=750&amp;s=66db3d2b">
              <source media="(min-width: 1690px)" srcset="//images.derstandard.at/img/2020/10/12/bluemel-002.jpg?w=265&amp;s=87892ac3">
              <source media="(min-width: 960px)" srcset="//images.derstandard.at/img/2020/10/12/bluemel-002.jpg?w=930&amp;s=386b862a">
              <img src="//images.derstandard.at/img/2020/10/12/bluemel-002.jpg?w=750&amp;s=66db3d2b" data-fullscreen-src="//images.derstandard.at/img/2020/10/12/bluemel-002.jpg?w=1600&amp;s=a57006fd">
            </picture>
          </figure>
          <header>
            <p class="teaser-kicker">Staatshaushalt <span>743</span></p>
            <h1 class="teaser-title">Wenig Investitionen, kaum Klimaschutz: Blümel erntet schon vor Rede Kritik für sein Budget</h1>
            <p class="teaser-subtitle">Der Finanzminister macht derzeit Unsummen für die Corona-Bekämpfung locker. Aus Sicht der Opposition geht die Strategie der Regierung aber nicht weit genug</p>
          </header>
        </div>
      </article>
    </section>
  </div>
</template>

<style lang="scss">
.frontpage {
}

.teaser {
  border-bottom: 1px solid rgba(0,0,0,0.1);

  > div {
    opacity: 0.6;

    img {
      filter: grayscale(100%);
    }
  }

  .teaser-kicker {
    text-transform: uppercase;
    font-family: $fs-condensed;
    margin: 0;
    font-size: 1.3rem;
  }

  .teaser-title {
    font-size: 1.8rem;
    margin: 4px 0 0;
  }

  .teaser-subtitle {
    font-size: 1.4rem;
    margin: 8px 0 0;
  }

  header {
    margin-top: 15px;
  }
}

.teaser > div,
.teaser-link {
  display: block;
  text-decoration: none;
  color: inherit;
  padding: 20px 25px;
}
</style>
