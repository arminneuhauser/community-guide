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
  height: 50px;
  display: flex;
  justify-content: space-between;
}
</style>
