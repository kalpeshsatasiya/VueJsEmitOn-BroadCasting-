<template>
  <div class="hello">
     <h3> Application footer title : {{ title }}</h3>
  </div>
</template>

<script>
import eventBus from './EventBus.vue';
export default {
  name: 'Footer',
  data(){
    return{
      title :"App"
    }
  },
  created(){
    eventBus.$on("changeTitle",(title)=>{this.title = title;})
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
