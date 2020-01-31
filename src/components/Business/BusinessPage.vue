<template>
<div class="BusinessPage">
    <div class="top">
       <input type="text"  placeholder="      search...." class="search">
    </div>
      <div class="side">
          <span class="page">Create a page</span><br>
          <input type="text" placeholder="create a page" class="createpage">
          <br><br> 
          CATEGEORIES:
          <select>
              <option selected>SPORTS</option>
              <option>BOLLYWOOD</option>
              <option>LIFE STYLE</option>
              <option>TECHNOLOGY</option>
              <option>FOOD</option>
          </select>
          <br>
          <br>
          <button>Create</button>
      </div>
    </div>
</template>
<script>
export default {
    name:'BusinessPage',
    data(){
        return{
          
        }
    }
}
</script>
<style scoped>
.top{
    height:200px;
}
.search{
    width:50%;
    height:50px;
    border-radius:10px;
    font-size:20px;
}
.side{
    float:left;
    font-size:20px;
    height:200px;
    border:2px solid black;
    box-shadow:2px 2px 2px 2px grey;
    margin-left:300px;
    width:60%;
}
.createpage{
    width:60%;
    height:30px;
    border-radius:10px;
} 
button{
    background-color: #3b5998;
    width:200px;
    height:40px;
    border-radius:20px;
    color:white;
    font-size:20px;
}
/* .page{
background: #3b5998;
} */
</style>