<template>
  <div class="hello">
      <h1 >{{ ce }}</h1>
      <div v-html = "parsed"></div>
    </div>
</template>


<script>
import katex from 'katex'
import 'katex/dist/contrib/mhchem'
import "katex/dist/katex.min.css"

export default {
  data () {
    return {
      ce: "\\ce{x Na(NH4)HPO4 ->[\\Delta] (NaPO3)_x + x NH3 ^ + x H2O}"
      }
  },
  computed: {
    parsed: function (){
      console.log("wrong"+this.ce)
      return katex.renderToString(this.ce, {displayMode: true})
    }
  },
  created () {
    console.log("abc"+this.ce)
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
