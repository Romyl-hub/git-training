<template>
 <div id="app"></div>
 <my-component/>
</template>

<script>
import MyComponent from './components/Mycomponent.vue'
import input from './components/input/input.vue'

export default {
  name: 'App',
  components: {
    MyComponent, 
    input
  }

}
</script>


