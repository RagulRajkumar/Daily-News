<template>
<div class="apps" id="apps">
  <Navbar/>
  <News/>
  <Footer/>
</div>
</template>

<script>
import News from './components/News.vue';
import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue';

export default {
  components: {
      News,
      Navbar,
      Footer
    },
  
};

</script>

<style>
html,body{
  width:100%;
}
#app{
  width: 100%;

}
.apps {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #ffffff;
  display:flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  margin:0px;
  padding: 0px;
  width:100%;
  background-color: #ffffff;  
}
h3{
  color:black;
}
/* width */
::-webkit-scrollbar {
   width: 5px;
 }
 
 /* Track */
 ::-webkit-scrollbar-track {
   background: #ffffff;
 }
 
 /* Handle */
 ::-webkit-scrollbar-thumb {
   background: #888;
   border-radius: 100px;
 }
 
 /* Handle on hover */
 ::-webkit-scrollbar-thumb:hover {
   background: #555;
 }
</style>
