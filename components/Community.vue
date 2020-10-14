<template>
  <section id="community" class="community">
    <header>
      <h1>{{this.headline}}</h1>
      <h2>Jeder User hat das Recht auf freie Meinungsäußerung.</h2>
    </header>
    <div v-if="this.moderation" class="moderation">
      <p>Dieses Forum wird moderiert von:</p>
      <div>
        <div class="guide">
          <strong>morgause</strong>
          <svg style="width:24px;height:24px" viewBox="0 0 24 24">
            <path fill="currentColor" d="M12,1L3,5V11C3,16.55 6.84,21.74 12,23C17.16,21.74 21,16.55 21,11V5L12,1M12,5A3,3 0 0,1 15,8A3,3 0 0,1 12,11A3,3 0 0,1 9,8A3,3 0 0,1 12,5M17.13,17C15.92,18.85 14.11,20.24 12,20.92C9.89,20.24 8.08,18.85 6.87,17C6.53,16.5 6.24,16 6,15.47C6,13.82 8.71,12.47 12,12.47C15.29,12.47 18,13.79 18,15.47C17.76,16 17.47,16.5 17.13,17Z" />
          </svg>
        </div>
        <div class="guide">
          <strong>Mostly Harmless</strong>
          <svg style="width:24px;height:24px" viewBox="0 0 24 24">
            <path fill="currentColor" d="M12,1L3,5V11C3,16.55 6.84,21.74 12,23C17.16,21.74 21,16.55 21,11V5L12,1M12,5A3,3 0 0,1 15,8A3,3 0 0,1 12,11A3,3 0 0,1 9,8A3,3 0 0,1 12,5M17.13,17C15.92,18.85 14.11,20.24 12,20.92C9.89,20.24 8.08,18.85 6.87,17C6.53,16.5 6.24,16 6,15.47C6,13.82 8.71,12.47 12,12.47C15.29,12.47 18,13.79 18,15.47C17.76,16 17.47,16.5 17.13,17Z" />
          </svg>
        </div>
        <div class="moderator">
          <strong>Rupert Böhler</strong>
          <svg style="width:24px;height:24px" viewBox="0 0 24 24">
            <path fill="currentColor" d="M12,1L3,5V11C3,16.55 6.84,21.74 12,23C17.16,21.74 21,16.55 21,11V5L12,1M12,5A3,3 0 0,1 15,8A3,3 0 0,1 12,11A3,3 0 0,1 9,8A3,3 0 0,1 12,5M17.13,17C15.92,18.85 14.11,20.24 12,20.92C9.89,20.24 8.08,18.85 6.87,17C6.53,16.5 6.24,16 6,15.47C6,13.82 8.71,12.47 12,12.47C15.29,12.47 18,13.79 18,15.47C17.76,16 17.47,16.5 17.13,17Z" />
          </svg>
        </div>
      </div>
    </div>
    <div class="top-posings">
      <h3>Welche dieser Postings möchtest du dem Forum voranstellen?</h3>
      <div class="postings">
        <posting v-for="item in items" :key="item.headline" :headline="item.headline" :message="item.message"/>
        <div class="success">
          <p>Vielen Dank für deine Auswahl.</p>
          <nuxt-link to="/story2">Weiter zum Artikel Wenig Investitionen, kaum Klimaschutz: Blümel erntet schon vor Rede Kritik für sein Budget</nuxt-link>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  props: [
    'moderation',
    'headline',
    'items'
  ]
}
</script>

<style lang="scss">
.community {
  header {
    background: var(--cta);
    color: var(--on-cta);
    padding: 8px 15px;

    h1, h2 {
      font-size: 1.3rem;
      font-weight: normal;
      margin: 0;
    }
  }
}

.success {
  background: green;
  padding: 15px;
  text-align: center;
  color: #fff;

  a {
    color: #fff;
  }
}

.posting {
  + .success {
    display: none;
  }
}

.moderation {
  > div {
    display: flex;
    flex-wrap: wrap;

    > div {
      display: flex;
      align-items: center;
      margin: 0 10px 5px 0;

      svg {
        margin-left: 3px;
      }
    }

    .guide {
      color: var(--guide);
    }

    .moderator {
      color: var(--cta);
    }
  }
}
</style>
