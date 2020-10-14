<template>
  <footer>
    <h2>© STANDARD Verlagsgesellschaft m.b.H. 2020</h2>
    <p>
      Alle Rechte vorbehalten. Nutzung ausschließlich für den privaten Eigenbedarf.<br>
      Eine Weiterverwendung und Reproduktion über den persönlichen Gebrauch hinaus ist nicht gestattet.
    </p>
    <pre>count: {{ $store.state.count }}</pre>
  </footer>
</template>

<script>
export default {
  data () {
    return {
      count: 0
    }
  }
}
</script>

<style lang="scss" scoped>
footer {
  font-size: 1.3rem;
  margin: 50px 0 30px;
  padding: var(--site-core-padding);

  * {
    opacity: 0.6;
  }

  h2 {
    font-size: 1.5rem;
  }

  pre {
    opacity: 0.12;
  }
}
</style>
