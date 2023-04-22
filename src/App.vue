<template>
  <div>
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

* {
  font-family: "RobotoRegular";
}

body {
  margin: 0;
}

#app {
  display: flex;
  flex-direction: column;
  height: 100vh;
  align-items: center;
  background: linear-gradient(to right, rgb(173, 169, 150), rgb(242, 242, 242), rgb(219, 219, 219), rgb(234, 234, 234));
}

</style>