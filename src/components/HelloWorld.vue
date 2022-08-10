<template>
  <div class="hello">
<!--     <h1>{{ msg }}</h1>
 -->

 <div>{{2 + 2}}</div>
 
  <div v-if="propertyShow">
      <h1>Enseña este si es true</h1>
    </div> 

    

    <h1 v-for="(post, index) in posts" :key="index">
      {{post.title}}
      {{post.description}}
      {{post.content}}
    </h1>
   
   </div>
   
  
</template>

<script>
export default {
  name: 'HelloWorld',
  data(){
    return{

      propertyShow: true,

       posts: [
      {title: "soy titulo 1",
      description: "Soy descriptción 1",
      content:"Malaga"
      },
      {title: "soy titulo 2",
      description: "Soy descriptción 2",
      content:"Barcelona"
      },
      {title: "soy titulo 3",
      description: "Soy descriptción 3",
      content:"Dubai"
      }
    ],

    

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
