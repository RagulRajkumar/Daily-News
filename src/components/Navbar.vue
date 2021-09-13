<template>
<div class="navbar">
    <ul>
        <h2 class="comp">Daily News</h2>
    </ul>
      
</div>
</template>
<script>

export default {
     name: 'Navbar',
}
</script>

<style>
.navbar {
  width: 100%;
  
}

ul {
  list-style-type: none;
  margin: 0px;
  padding: 10px;
  overflow: hidden;
  background-color: #333;
}
h2 {
  float: center;
  margin: 10px;
}
h2 a{
  color: white;
  text-decoration: none;
}
</style>