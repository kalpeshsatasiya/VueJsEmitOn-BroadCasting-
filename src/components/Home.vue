<template>
  <div class="hello">
    <Header/>
     <h1> VueJs (Broadcast) Emit-On Demo</h1>        
    
    <Footer/>
  </div>
</template>

<script>
import Header from './Header.vue'
import Footer from './Footer.vue'

export default {
  name: 'Home',
  components: {
    Header,
    Footer
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
