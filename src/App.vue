<template>
  <div id="app">
    <Parallax class="first-scene" :parallax="true"
    :directon="down" :speedFactor="0.15">
      <h1 id="title-one">Hello World</h1>
      <img class="img1" src="./assets/moon.jpg" alt="">
    </Parallax>
   <Parallax :parallax="true" :direction="up" :speedFactor="0.15">
    <div class="container2">
      <h1 id="third-title">Bye World</h1>
    </div>
      <img src="./assets/land.jpg" class="img2" alt="">
    </Parallax>
  </div>
</template>

<script>
import Parallax from 'vue-parallaxy';

export default {
  name: 'App',
  components: {
    Parallax
  },
}
</script>

<style>
*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

.first-scene{
  display: flex;
  align-items: center;
  justify-content: center;
}

#title-one{
  position: absolute;
  color: white;
  font-family: sans-serif;
  font-size: 90px;
}

#third-title{
  position: absolute;
  color: white;
  font-family: sans-serif;
  font-size: 85px;
}

.container2{
  display: flex;
  flex-direction: row;
  justify-content: center;
}

</style>
