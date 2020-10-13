<template>
  <section class="community">
    <header>
      <h1>1.163 Postings</h1>
      <h2>Jeder User hat das Recht auf freie Meinungsäußerung.</h2>
    </header>
    <div>
      <h3>Wählen Sie Top-Postings aus:</h3>
      <div>
        <posting v-for="item in items" :key="item.message" :headline="item.headline" :message="item.message"/>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data () {
    return {
      items: [
        {
          headline: 'Foo',
          message: 'Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.'
        },
        {
          headline: 'Bar',
          message: 'Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.'
        }
      ]
    }
  }
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
</style>
