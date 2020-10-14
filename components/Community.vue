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
    <div class="top-postings">
      <posting v-for="item in toppostings" :key="item.headline" :user="item.user" :headline="item.headline" :message="item.message" :actions="false"/>
    </div>
    <div id="rate-postings" class="rate-postings">
      <h3>Welche dieser Postings möchtest du dem Forum voranstellen?</h3>
      <div class="postings">
        <posting v-for="item in items" :key="item.headline" :headline="item.headline" :message="item.message" :actions="true"/>
        <div class="success">
          <p>Vielen Dank für deine Auswahl.</p>
          <p><nuxt-link to="/story2#community">Weitere Postings auswählen im Artikel Blümel erntet schon vor Rede Kritik für sein Budget</nuxt-link></p>
        </div>
      </div>
    </div>
    <div class="forum">
      <div class="forum-input">
        <svg style="width:24px;height:24px" viewBox="0 0 24 24">
          <path fill="currentColor" d="M10,9V5L3,12L10,19V14.9C15,14.9 18.5,16.5 21,20C20,15 17,10 10,9Z" />
        </svg>
        <p>Ihr Kommentar</p>
      </div>
      <div class="upost" v-for="index in 10" :key="index">
        <div class="upost-header">
          <span>Username</span>
          <small>vor x Stunden</small>
        </div>
        <div class="upost-content">
          Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam
        </div>
        <div class="upost-footer">
          <a href="#">antworten</a>
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
    'items',
    'toppostings'
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
      text-transform: none;
    }
  }
}

.success {
  background: green;
  padding: 15px;
  text-align: center;
  color: #fff;
  margin-bottom: 20px;

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
  > p {
    margin: 15px 0 10px;
  }

  > div {
    display: flex;
    flex-wrap: wrap;
    margin-bottom: 15px;

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

.forum {
  .forum-input {
    @include box-shadow;
    background: #fff;
    padding: 10px 15px 40px;
    display: flex;
    align-items: center;

    * {
      opacity: 0.6;
      margin: 0;
    }

    svg {
      transform: rotate(180deg);
      margin-right: 5px;
    }
  }
}

.upost {
  background: var(--border-color);
  margin: 10px 0;
  opacity: 0.4;

  .upost-header {
    font-size: 1.2rem;
    background: rgba(0,0,0,0.1);
    padding: 5px 10px;
    border-bottom: 1px solid rgba(0,0,0,0.1);
  }

  .upost-content {
    font-size: 1.5rem;
    padding: 5px 10px;
  }

  .upost-footer {
    border-top: 1px solid rgba(0,0,0,0.1);
    padding: 5px 10px;
    font-size: 1.3rem;

    a {
      color: inherit;
      opacity: 0.6;
    }
  }
}
</style>
