<template>
  <div class="backdrop">
    <div class="modal">
      <svg viewBox="0 0 24 24">
        <path fill="currentColor" d="M18 2C17.1 2 16 3 16 4H8C8 3 6.9 2 6 2H2V11C2 12 3 13 4 13H6.2C6.6 15 7.9 16.7 11 17V19.08C8 19.54 8 22 8 22H16C16 22 16 19.54 13 19.08V17C16.1 16.7 17.4 15 17.8 13H20C21 13 22 12 22 11V2H18M6 11H4V4H6V11M20 11H18V4H20V11Z" />
      </svg>
      <h1>Gratulation!</h1>
      <p>Du hast 5 Postings bearbeitet. Als Dankeschön erhältst du 3 Monate PUR gratis.</p>
      <p>
        <nuxt-link class="button" to="/pur">Jetzt einlösen</nuxt-link>
      </p>
    </div>
  </div>
</template>

<style lang="scss">
.backdrop {
  position: fixed;
  width: 100vw;
  height: 100vh;
  background: rgba(0,0,0,0.5);
  top: 0;
  left: 0;
  padding: 25px;
  z-index: 3;
  display: flex;
  align-items: center;
  justify-content: center;
}

.modal {
  background: var(--background);
  max-width: 350px;
  padding: 25px;
  text-align: center;

  svg {
    width: 48px;
    height: 48px;
  }

  h1, p {
    margin: 10px 0;
  }
}
</style>
