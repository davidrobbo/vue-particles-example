<template>
  <div class="hello">
    <div class="particle-outer">
      <vue-particles
              color="#dedede"
              :particleOpacity="0.7"
              :particlesNumber="180"
              shapeType="circle"
              :particleSize="4"
              linesColor="#dedede"
              :linesWidth="1"
              :lineLinked="true"
              :lineOpacity="0.4"
              :linesDistance="150"
              :moveSpeed="3"
              :hoverEffect="true"
              hoverMode="grab"
              :clickEffect="true"
              clickMode="push"
      >
      </vue-particles>
    </div>
  </div>
</template>

<script>
import Vue from 'vue'
import VueParticles from 'vue-particles'
Vue.use(VueParticles)
export default {
  name: 'hello',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
.hello {
  background: url('/static/img.jpg') no-repeat;
  background-size: cover;
  position: fixed;
  height: 100%;
  width: 100%;
  top:0;
  left:0;
}
.particle-outer {
  background: #000;
  opacity: 0.5;
}
</style>
