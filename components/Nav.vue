<template>
  <div class="nav">
       <div class="container">
     <nav class="navbar navbar-expand-md navbar-light">
  <div class="collapse navbar-collapse" id="navbarSupportedContent">
         <ul class="navbar-nav">
           <li class="nav-item"> <router-link to="/"><span>Home</span></router-link></li>
           <li class="nav-item"><router-link to="/register">Rgister</router-link></li>

        </ul>

  </div>

     </nav>

    </div>
  
          </div>
</template>

<script>
export default {

}
</script>

<style>
.nav
{
    background-image: url("~/assets/images/download.jpg");
 background-size: cover;
 height: 250px;
}
.navbar-expand-md .navbar-collapse
{
    padding-left: 40%;
    padding-top: 50px;
}
span
{
    color: darkred;
    
}
.navbar-nav{
    text-align: center;
    background-color:#fff;
    border-radius: 20px;
    padding-left: 70px;
    /* padding-right: 70px; */
    padding-top: 15px;
    padding-bottom: 15px;
    font-weight: bold;

}
.nav-item{
  padding-left: 15px;;
  text-align: center;
}
a
{
  color: #000;
  
}
a:hover
{
text-decoration: none;
color:maroon;
}
.navbar-expand-md .navbar-nav
{
  padding-right: 20px;
  padding-left: 20px;

}

</style>