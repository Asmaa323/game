<template>
<div>
    <section>
        <TowMenu/>
            
    <div class="container" style="padding-left:20%;">
        <div class="card border-2 shadow-lg "  style="width:500px;">
            <div class="header">
                Register
            </div>
            <p class="text-register ">Before signing up, please read through the <span class="span-zero">manual</span> 
                in order to gain a better understanding of the advantages 
                and disadvantages of the three tribes.</p>
            <div class="card-body">
            
        <form method="post" action="/register" @submit.prevent="OnSubmit">
    
  <div class="form-group">
      <label for="nickname">Nicename address</label>
    <input type="nickname" id="nickname" aria-describedby="nicknameHelp" placeholder="Enter NickName" v-model="form.nickname">
    <br>
    <label for="exampleInputEmail1">E-mail</label>
    <input type="email" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="Enter email" v-model="form.email">
    <br>
    <label for="exampleInputPassword1">Password</label>
    <input type="password"  id="exampleInputPassword1" placeholder="Password" v-model="form.password">
  </div>
  <div class="all-radio">
  <label class="name-label">
      
أختر القبيلة</label>
<br>
  <div class="form-check form-check-inline">
       <div class="name-radio">
  <input class="form-check-input" value="
 الرومان" type="radio" name="flexRadioDefault" id="flexRadioDefault1" v-model="form.radio">
  <label class="form-check-label" for="flexRadioDefault1">
 الرومان
  </label>
       </div>
        <div class="name-radio">

  <input class="form-check-input" type="radio" value=" العرب" name="flexRadioDefault" id="flexRadioDefault2" checked  v-model="form.radio">
  <label class="form-check-label" for="flexRadioDefault2">
    العرب
  </label>
        </div>
         <div class="name-radio">

  <input class="form-check-input" type="radio" value="الجرمان" name="flexRadioDefault" id="flexRadioDefault3" checked  v-model="form.radio">
  <label class="form-check-label" for="flexRadioDefault3">
  الجرمان
  </label>
         </div>
  </div>
  <br>
  <div class="form-check form-check-inline">
      <div class="name-radio">
  <input class="form-check-input" value="الفراعنة" type="radio" name="flexRadioDefault" id="flexRadioDefault4" checked  v-model="form.radio">
  <label class="form-check-label" for="flexRadioDefault4">
   الفراعنة
  </label>
      </div>
 <div class="name-radio">
  <input class="form-check-input" value=" الإغريق" type="radio" name="flexRadioDefault" id="flexRadioDefault4" checked  v-model="form.radio">
  <label class="form-check-label" for="flexRadioDefault4">
    الإغريق
  </label>
 </div>
  <div class="name-radio">
  <input class="form-check-input" value="المغول" type="radio" name="flexRadioDefault" id="flexRadioDefault4" checked  v-model="form.radio">
  <label class="form-check-label" for="flexRadioDefault4">
المغول  </label>
  </div>
</div>
  </div>

<br>
 <div class="name-radio">
    <input class="form-check-input" type="checkbox" value="" id="flexCheckDefault" v-model="form.checkbox">
  <label class="form-check-label" for="flexCheckDefault">
      I accept Rule and Privacy .
  </label>
 </div>
  <div class="btn-submit" >
  <button type="submit" class="btn btn-primary " >Submit</button>
  </div>
</form>
        </div>
        </div>

        </div>
    </section>
    </div>
    
</template>
<style scoped>
section
{
    box-shadow: 20px;
   
    padding-top: 50px;

}

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
            a:hover
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

.header
{
     text-align: center;
    font-style:italic;
    font-size: 20px;
    padding-bottom: 20px;
}
button
{

    border-radius: 50px;
    background: #808B97;
    width: 100px;
    border: #808B97;
    text-align: center;
    
}
div .name-label
{
    text-align: left;
    color: darkorange;
}
button:hover
{
 border:2px solid chartreuse;
  background: #808B97;
   text-align: center;
}
.name-radio
{
    padding-left: 50px;
    padding-top: 20px;
    padding-bottom: 20px;
     text-align: center;
}
.all-radio
{
        outline: thin dotted;
  outline-offset: -2px;

}
.text-register
{
    font-size: 20px;
    text-align: center;
    margin-left: 20px;
    text-align: left;

}
.span-zero
{
    color:chartreuse;

}
.span-zero:hover{
    color: darkgreen;
}
input
{
 
  box-shadow: none;
  border:2px solid yellowgreen;
  

}
.form-group
{
    padding-top:20px;
       outline: thin dotted;
  outline-offset: -2px;
  padding-bottom: 20px;
  text-align: left;
  padding-left: 20px;
  font-weight: bold;
}

input:hover
{
   border-color: black;


}
.btn-submit
{
    text-align: center;
}

</style>
<script>
import Nav from '../components/Nav.vue';
import TowMenu from'../components/TwoMenu.vue'
export default {
  components: { Nav ,TowMenu},
    name:"register",
    layout:"empty",
    data()
    {
        return{
            form:{
                nickname:"",
                email:"",
                password:"",
                radio:"",
                checkbox:""



            }
        }
    },
    methods:
    {
        OnSubmit()
        {
         this.$axios.post('/register',{
             nickname:this.form.nickname,
             email:this.form.email,
             password:this.form.password,
             radio:this.form.radio,
             checkbox:this.form.checkbox

         
         }).then(data=>{
            this.$swal(
  'Good job',
  'You clicked the button!',
  'success'
)
         });
    
           
        }
    }

}
</script>



