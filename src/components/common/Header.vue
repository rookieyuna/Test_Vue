<template>
  <header>
    <h1><router-link to="/"><a href="#" class="logo"><img alt="Vue Logo" src="../../assets/logo.png" width="80"></a></router-link></h1>
    <nav>  
    <ul class="menu">
        <li><router-link to="/about"><a href="javascript:;">게시판</a></router-link></li>
        <li><a href="javascript:;">메뉴2</a></li>
        <li><a href="javascript:;">메뉴3</a></li>
        <li><a href="javascript:;">메뉴4</a></li>
    </ul>
    </nav>
  </header>
</template>

<script lang="ts">
export default {

}
</script>

<style scoped>
header {
    width: 100%;
    text-align: center;
    /* position: relative; */
    height: 120px;
    border-bottom: 1px solid #35495e;
}
header h1 {
    position: absolute;
    top: 0;
    left: 100px;
}
header ul.menu:after{
    display: block;
    clear: both;
    content: '';
}
header ul.menu {
    position: absolute;
    top: 20px;
    right: 50px;
}
header ul.menu li{
    float:left; 
    padding:10px 20px; 
    list-style:none;
}

a {
    text-decoration:none; 
    color:rgb(2, 73, 0);
}

</style>