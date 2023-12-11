<template>
  <header class="site clearfix">
    <div class="col one">
      <img class="logo" src="@/assets/Harry.png" alt="HMaxWilson" width="280" height="373" />
    </div>
    <div class="col two">
      <h4>Astro Systems (tm) <br /> <b>W</b>ireless <b>I</b>dentity and <b>L</b>ogistical <b>S</b>ecurity <b>O</b>perating <b>N</b>ode (WILSON)</h4>
      <p class="hidden lg:block">-------------------------------------------</p>
      <p class="block lg:hidden">------------------</p>
      <p>WILSON v1.0.0</p>
      <p>(c){{ currentDate.getFullYear() }} - AstroNomad Design</p>
    </div>
  </header>
</template>

<script setup>
  const currentDate = new Date();
</script>

<style scoped>
header.site {
  margin: 0 0 40px 0;
  text-transform: uppercase;
}
.col {
  float: left;
  padding: 0 20px;
}
.col.two {
  width: auto;
}
#logo-v {
  display: block;
  height: auto;
  margin: 0 auto;
  width: 260px;
}
</style>