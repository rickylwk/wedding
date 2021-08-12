<template lang="pug">
h1#fade Monse & Ricky
<div class="nav-item"><a href="#">Our Story</a></div>
<div class="nav-item"><a href="#">Gallery</a></div>
<div class="nav-item"><a href="#">Food Menu</a></div>
<div class="nav-item"><a href="#">Direction</a></div>
<div class="circle"><a href="#">circle</a></div>

</template>

<script>
import { gsap } from "gsap";

export default {
  name: 'App',
  mounted: function(){
    gsap.to('.circle', {x: 500, duration: 3})
  }
}

</script>

<style scoped lang="scss">
@import "assets/css/normalize.css";
@import "assets/css/common.scss";

.circle{
  background-color:red;
  height: 5em;
  width: 5em;
  border-radius: 100%
}

</style>
