<template>
 <div class="container" style="padding-left:20%; margin-top:-36px;">
        <div class="card border-2 shadow-lg "  style="width:600px;">
            <div class="header ml-auto">
         Welcome to the Tatar war
            </div>
            <p class="text-index">  It is a free browsing game that doesn't need to be downloaded, a war game in a world full of real players who all start out as the leaders of small villages
</p>
<div class="header ml-auto">
    about the game
</div>
<span class="line"></span>
        
                <ul>
                    <li class="text-one "> Number of players: 3376</li>
                    <li class="text-one ">Currently online: 308
</li>
                    <li class="text-one">Number of servers: 6</li>
                    <li class="text-one">You will start out as the head of a small village.
</li>
                    <li class="text-one">You will develop buildings, fields and army.
</li>
                    <li class="text-one">You will fight with or against real players.
</li>
                </ul>
                <div class="header ml-auto">
                Shots
            </div>

            <span class="line"></span>
            <!-- //////////////////////////////////////////////////////////////////////////////// -->
    <div class="global-model">

  <b-img class="model-image"  v-b-modal.modal-1 src="~/assets/images/download.jpg" />

  <b-modal class="model" id="modal-1" title="buildings">
    <div class="text-model my-4">
    
        <b-img v-b-modal.modal-1 src="~/assets/images/download.jpg" width="450px" height="200px"/>
            
    </div>

  </b-modal>


  <b-img class="model-image"  v-b-modal.modal-2 src="~/assets/images/download.jpg"/>

  <b-modal class="model" id="modal-2" title="Fileds">
       <div class="text-model my-4">
        <b-img v-b-modal.modal-1 src="~/assets/images/download.jpg" width="450px" height="200px"/>
            
    </div>
  </b-modal>


  <b-img class="model-image"  v-b-modal.modal-3 src="~/assets/images/download.jpg" />

  <b-modal class="model" id="modal-3" title="the map">
         <div class="text-model my-4">
        <b-img v-b-modal.modal-1 src="~/assets/images/download.jpg" width="450px" height="200px"/>
            
    </div>

  </b-modal>



  <b-img class="model-image" v-b-modal.modal-4 src="~/assets/images/download.jpg"  />

  <b-modal class="model" id="modal-4" title="gold">
      <div class="text-model my-4">
        <b-img v-b-modal.modal-1 src="~/assets/images/download.jpg" width="450px" height="200px"/>
            
    </div>

  </b-modal>
</div>

    </div>




            </div>
        
</template>

<style scoped>
.header
{
    font-size: 20px;
    padding-bottom: 20px;
    font-weight: bold;
    

}
.global-model
{
    text-align: center;
    padding-top: 20px;
    
}
.model-image{
    padding-left: 10px;
    padding-right: 10px;
    width: 100px;
    height: 100px;
    border: 2px solid black;
}
.model-image:hover{
    opacity: 0.5;
}
/* .text-model
{
    background-image: url("~/assets/images/download.jpg");
} */
/* .model
{
width: 200px;
height: 200px;;    
} */
.link-header
{
    color: green;
    font-weight: bold;
    cursor: pointer;

}
.text-index
{
    padding: 10px 10px;

}
.line {
                      outline: thin dotted;
                        outline-offset: 2;
  color: darkgray;
  margin-left: 20px;
  margin-right: 20px;

}

</style>
<script>
export default {
  

}
</script>
