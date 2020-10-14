<template>
  <div v-if="this.active" class="posting">
    <div class="posting__body">
      <h4>{{ headline }}</h4>
      <p>{{ message }}</p>
    </div>
    <div v-if="actions" class="posting__actions">
      <div>
        <button @click="onClick">
          <svg style="width:24px;height:24px" viewBox="0 0 24 24">
            <path fill="currentColor" d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" />
          </svg>
          <!--<span>Ablehnen</span>-->
        </button>
      </div>
      <div>
        <button @click="reportVisible = !reportVisible">
          <svg style="width:24px;height:24px" viewBox="0 0 24 24">
            <path fill="currentColor" d="M14.4,6L14,4H5V21H7V14H12.6L13,16H20V6H14.4Z" />
          </svg>
          <!--<span>Melden</span>-->
        </button>
        <div v-show="reportVisible" class="report">
          <input type="text" placeholder="Ihr Name">
          <input type="email" placeholder="Ihre E-Mail-Adresse">
          <textarea placeholder="Begründung"></textarea>
          <button @click="onClick(); reportVisible = false" class="button">Absenden</button>
          <button @click="reportVisible = false">Abbrechen</button>
        </div>
      </div>
      <div>
        <button @click="onClick">
          <svg style="width:24px;height:24px" viewBox="0 0 24 24">
            <path fill="currentColor" d="M9,20.42L2.79,14.21L5.62,11.38L9,14.77L18.88,4.88L21.71,7.71L9,20.42Z" />
          </svg>
          <!--<span>Auswählen</span>-->
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      active: true,
      reportVisible: false
    }
  },
  props: [
    'headline',
    'message',
    'actions'
  ],
  computed: {
    count () {
      return this.$store.state.count
    }
  },
  methods: {
    onClick: function() {
      this.active = false

      this.$store.commit('increment')
    }
  }
}
</script>

<style lang="scss">
.posting {
  background: var(--posting-background);
  border: 1px solid var(--border-color);
  margin-bottom: 15px;
  font-size: 1.5rem;

  .posting__body {
    padding: 15px;

    h4, p {
      margin: 0 0 6px;
    }
  }

  .posting__actions {
    border-top: 1px solid var(--border-color);
    display: flex;

    > div {
      position: relative;
      flex-grow: 1;

      &:nth-child(2) {
        border-width: 0 1px;
        border-color: var(--border-color);
        border-style: solid;
      }

      > button {
        border: 0;
        background: 0;
        height: 35px;
        line-height: 0;
        width: 100%;
        display: flex;
        align-items: center;
        justify-content: center;

        span {
          font-size: 1.3rem;
          font-weight: bold;
          margin-left: 5px;
        }
      }
    }
  }

  .report {
    @include box-shadow;

    position: absolute;
    background: #fff;
    width: 60vw;
    max-width: 350px;
    left: 0;
    bottom: 100%;
    padding: 15px;
    display: flex;
    flex-direction: column;
    transform: translateX(-25%);

    input, textarea, button {
      width: 100%;
      margin-bottom: 10px;
    }

    textarea {
      min-height: 80px;
    }

    button:not(.button) {
      border: none;
      background: none;
      margin: 0;
    }
  }
}
</style>
