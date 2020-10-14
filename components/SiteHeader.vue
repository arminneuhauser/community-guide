<template>
  <header>
    <logo/>
    <notifications/>
  </header>
</template>

<style lang="scss" scoped>
header {
  @include box-shadow;

  position: fixed;
  background: var(--background);
  top: 0;
  left: 0;
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  z-index: 1;

  @include breakpoint(l) {
    padding: 10px;
  }
}
</style>
