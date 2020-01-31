<template>
  <div>
    <h1>REGISTER</h1>
    <div class="register">
      <form>
          <div>
        <div class="inputfield">
            <label>NAME:</label>
            <input type="text" placeholder="NAME" v-model="name" 
            required/><br><br>
        </div>
        <div class="inputfield">
            <label>E-MAIL:</label>
            <input type="email" placeholder="E-mail" v-model="email" required/><br><br>
        </div>
        <div class="inputfield">
            <label>MOBILE NUMBER</label>
            <input type="number" placeholder="CONTACT" v-model="mobilenumber" required/><br><br>
        </div>
        <div class="inputfield">
          <label>GENDER</label>
          <select>
            <option>MALE</option>
            <option>FEMALE</option>
          </select>
        </div>
        <div class="inputfield">
        <label>DOB:</label>
        <input type="date" v-model="date" required><br><br>
        </div>
        <div class="inputfield">
        <label>ROLE</label>
        <select @click="disable">
          <option selected>USER</option>
          <option id="business">BUSINESS</option>
        </select><br><br>
        </div>
        <div class="inputfield">
        <label>PROFILE TYPE</label>
        <select id="typed">
          <option selected>PUBLIC</option>
          <option>PRIVATE</option>
        </select><br><br>
        </div>
        <div class="inputfield">
        <label>INTERESTS</label>
        <select>
          <option selected>SPORTS</option>
          <option>BOLLYWOOD</option>
          <option>LIFE STYLE</option>
          <option>TECHNOLOGY</option>
          <option>FOOD</option>
        </select>
        </div>
        <button>REGISTER</button>
        </div>
      </form>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
       name:'',
      email:'',
      mobilenumber:'',
      date:'',

    };
  },
  // methods:{
  //   disable:function(){
  //     if(document.getElementById('business'))
  //     {
  //     return document.getElementById('typed').options[1].disabled= true;
  //     }
  //     else{
  //       return document.getElementById('typed').options[1].disabled= false;
  //     }
  //   }
  //  }
};
</script>
<style scoped>
.inputfield{
  height:50px;
}
h1 {
  margin: 0 auto;
  background-color: #3b5998;
  width: 680px;
  color: white;
}
.register {
  width: 38%;
  margin: 0 auto;
  border: 2px solid black;
  padding: 5%;
  font-family: sans-serif;
}
input ,select{
  height:30px;
  float:right;
  width:250px;
  margin-right:30px;
}
button {
  width: 200px;
  border-radius: 50px;
  height: 30px;
  background-color: #3b5998;
  color: white;
  font-size: 20px;
  margin: 30px;
}
label {
  float:left;
  font-size:15px;
  font-family: sans-serif;
}
</style>