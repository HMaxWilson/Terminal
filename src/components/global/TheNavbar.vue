<template>
  <nav class="site clear">
    <ul>
      <li><a href="/" title="">Home</a></li>
      <li><a href="/about" title="">Misc</a></li>
    </ul>
  </nav>
</template>

<style scoped>
nav.site {
  margin: 0 0 40px 0;
  position: relative;
  width: 100%;
  z-index: 10;
}

nav.site ul {
  padding: 0;
}

nav.site ul li {
  display: inline-block;
  padding: 0 10px;
  min-width: 120px;
  width: auto;
}
</style>