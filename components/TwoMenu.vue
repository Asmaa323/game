<template>
  <div>
      <div class="leftDiv">
                                 <div class="col-md-10 col-xs-12">

                                     <div >
                                         <a class="name-home" href="/">Home</a><br>
                                         <a class="name-home" href="/">Help</a><br>
                                         <a  class="name-home" href="/">Sign In</a><br>
                                         <a class="name-home" href="/">Sign Up</a><br>
                                     </div>
                                     
                       <!-- <i class="flag flag-united-states"></i>
                       <span class="flag-icon flag-icon-us"></span>
                       <span class="flag-icon flag-icon-gr flag-icon-squared">Asmaa</span> -->
                       
                                        
                     
                    
                </div>

     
            </div>
            <div class="rightDiv">
           <span class="span-one">    The official site of the Tatar war</span> <br>

We are here to compete in the world of the Tatar war and get to know each other our skills in combat and planning.

<br><span class="span-two"> Compete to build the miracle</span><br>

with all due respect
            </div>
  </div>
</template>

<script>
export default {
  name:"twomenu"

}
</script>

<style>

   .leftDiv {
                background-color: #fff;
                color: #000;
                height: 400px;
                width: 28%;
                float: left;
                text-align: center;
               
            }
            .name-home
            {
                padding-bottom: 30px;
                font-weight: bold;
                padding-top: 20px;
              
            }
            .name-home:hover
            {
                color: chartreuse;
                    outline: thin dotted;
  outline-offset: -2px;
  padding: 10px 10px 10px 10px;
            }
            
            .rightDiv {
                background-color: #fff;
                color: #000;
                height: 250px;
                width: 18%;
                float: right;
                text-align: left;
                       outline: thin dotted;
  outline-offset: -2px;
                
            }
            .span-one
            {
                color: chartreuse;
                font-size: 20px;
            }
            .span-two
            {
                color: red;
                
               

            }
</style>