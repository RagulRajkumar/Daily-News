<template>
<div class="new" id="new">
  <div v-for="article in articles" :key="article">
    <n-card >
    <template #cover>
      <a
      :href="article.url"
       target="_blank" 
       style="text-decoration:none;color:black;">
        <img class="image" :src="article.urlToImage" />
      <h4>{{article.title}}</h4>
       </a>
    </template>
  </n-card>
  </div>
</div>
</template>

<script>
import { NCard } from 'naive-ui'

export default {
    name:'Business',
  components: {
      NCard
    },
  data:function(){
    return{
      articles:[]
    }
  },
   mounted: function () {
     var that = this;
    var url =
     'https://newsapi.org/v2/top-headlines?country=in&category=business&apiKey=3ee26f40f19147938b15e9662e597ea9';

    var req = new Request(url);

    fetch(req).then(function (response) {
      return response.json();
    })
    .then(function(data){
      console.log(data);
      that.articles = data.articles;
    });
  },
};

</script>

<style>
#new {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #ffffff;
  display:flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  background-color: #ffffff;  
  overflow-y: scroll;
}
.n-card {
  width: 250px;
  margin: 30px;
  height: 300px;
  cursor: pointer;
}
.image{
  height: 200px;
}
</style>
