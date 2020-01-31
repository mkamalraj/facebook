<template>
  <div class="posting">
    <h1 class="heading">CREATE POST</h1>
    <input type="text" class="box" placeholder="   WRITE SOMETHING HERE    "/>
    <div class="right">
      <button>UploadImage</button>
      <button>UploadVideo</button>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {

    };
  },
};
</script>
<style scoped>
.posting{
    width:60%;
    margin-left:100px;
    height:300px;
    box-shadow: 3px 2px 2px 5px  #888888;
}
.box{
  margin-top:30px;
  height: 50px;
  width:30%;
  border-radius: 50px;
  border: 2px solid black;
  background-color: rgba(220, 237, 242,0.2);
  font-size:20px;
  color:white;
}
.right {
  padding-top:10px;
  float: right;
  display:flex;
  flex-direction: column;
}
button {
  padding:5px;
  border-radius: 10px;
  margin:10px;
}
.heading{
  background-color:  rgba(33, 168, 209);
  width:100%;
  height:50px;
  border-bottom:2px solid black;
}
</style>