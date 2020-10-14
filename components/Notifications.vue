<template>
  <div class="notifications" v-click-outside="hide">
    <button @click="showNotifications = !showNotifications">
      <div>
        <span>{{ items.length }}</span>
      </div>
      <svg style="width:24px;height:24px" viewBox="0 0 24 24">
        <path fill="currentColor" d="M21,19V20H3V19L5,17V11C5,7.9 7.03,5.17 10,4.29C10,4.19 10,4.1 10,4A2,2 0 0,1 12,2A2,2 0 0,1 14,4C14,4.1 14,4.19 14,4.29C16.97,5.17 19,7.9 19,11V17L21,19M14,21A2,2 0 0,1 12,23A2,2 0 0,1 10,21" />
      </svg>
    </button>
    <nav v-if="showNotifications">
      <nuxt-link to="/story#community" v-for="item in items" :key="item.message" @click.native="showNotifications = false">
        <p v-html="item.message"></p>
        <p><small>{{ item.timestamp }}</small></p>
      </nuxt-link>
    </nav>
  </div>
</template>

<script>
export default {
  data () {
    return {
      showNotifications: false,
      items: [
        /*{
          message: 'Gratulation! Du hast 1.000 Postings bearbeitet. Als Dankeschön erhältst du 3 Monate PUR gratis.<br><strong><u>Jetzt einlösen</u></strong>',
          timestamp: 'vor 4 Stunden'
        },*/
        {
          message: 'Username, schön, dass du da bist. Wähle für den Artikel <strong>Grüner Unterwerfungsprozess</strong> interessante Stimmen aus dem Forum aus!',
          timestamp: 'vor 2 Stunden'
        }
      ]
    }
  },
  methods: {
    hide: function() {
    	this.showNotifications = false;
    }
  }
}
</script>

<style lang="scss" scoped>
.notifications {
  position: relative;

  button {
    border: 0;
    background: none;
    display: flex;
    padding: 13px;
    position: relative;

    > div {
      position: absolute;
      top: 10px;
      right: 10px;
      width: 12px;
      height: 12px;
      background: var(--cta);
      border-radius: 100%;
      border: 2px solid var(--background);

      span {
        @include visually-hidden;
      }
    }
  }

  nav {
    @include box-shadow;

    position: absolute;
    right: 10px;
    width: calc(100vw - 20px);
    background: var(--background);
    z-index: 2;

    a {
      color: inherit;
      border-bottom: 1px solid var(--border-color);
      padding: 10px;
      text-decoration: none;
      display: block;

      &:last-child {
        border: 0;
      }
    }

    p {
      font-size: 1.4rem;
      margin: 0;
    }

    small {
      opacity: 0.6;
    }
  }
}
</style>
