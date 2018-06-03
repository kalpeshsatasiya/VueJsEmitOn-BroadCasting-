<template>
  <div class="hello">
    <h3> Application header title : {{ title }}</h3>
    <input type="button" v-on:click="changeTitle" value="Ok" />
  </div>
</template>

<script>
import eventBus from './EventBus.vue';
export default {
  name: 'Header',
  data(){
    return {
      title : "App"
    }
  },
  methods: {
    changeTitle(){
      this.title ="Emit-On Demo";
      eventBus.$emit("changeTitle","Emit-On Demo");
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
</style>
