<template>

  <div class="container">
    <div id='app'>
      <logo/>
      <h1 class="title">
        {{title}} in Bed and Breaksfast
      </h1>
      <h2>Lingua corrente  {{$i18n.locale}}</h2>
      <no-ssr><div>dimensione corrente {{ $mq }}</div></no-ssr>
   
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})

</script>

<script>
 new Vue({
   el: '#app',
   data: {
     title: 'bevenuto'
   }
 })
</script>


<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
