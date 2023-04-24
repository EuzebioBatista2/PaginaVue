<template>
  <div class="app">
    <Display />
  </div>
</template>

<script>
import Display from './components/Display.vue'
export default {
  components: { Display }

}
</script>

<style>
@font-face {
  font-family: "RobotoRegular";
  src: url('./fonts/Roboto-Regular.ttf');
}

html {
  font-size: 62.5%;
}

* {
  font-family: "RobotoRegular";
}

body {
  margin: 0;
  padding: 0;
  background: linear-gradient(to right, rgb(173, 169, 150), rgb(242, 242, 242), rgb(219, 219, 219), rgb(234, 234, 234));
}

.app {
  padding: 50px;
}
</style>