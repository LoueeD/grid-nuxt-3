<template>
  <div class="sitenav">
    <GridfoxLogo />
  </div>
</template>

<style scoped lang="scss">
.sitenav {
  position: sticky;
  top: 0;
  height: 46px;
  background: #fff;
  border-bottom: 1px solid rgba(#111, 0.1);
  display: flex;
  z-index: 50;

  :deep(svg) {
    width: 20px;
  }
}
</style>
