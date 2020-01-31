<template>
  <div class="Friends">
      FRIENDS
    <div v-for="(items,index) in profiles" :key="index" class="list">
      <table>
        <tr>
          <td>
            <img v-bind:src="items.image" class="image" />
          </td>
          <td>&nbsp;&nbsp;&nbsp;
              {{items.name}}
          </td>
          <td>
            <button @click="addFriend"  id="myButton1" value="Add Friend">Add Friend</button>
          </td>
        </tr>
      </table>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      profiles: [
        {
          image:
            "https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRa7q8XhBB5inHO3kZa7CMM3NLEnAiVmgxTChTdxorZeVPQRRPu",
          name: "SOHAIL"
        },
        {
          image:
            "https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRa7q8XhBB5inHO3kZa7CMM3NLEnAiVmgxTChTdxorZeVPQRRPu",
          name: "NAVEEN"
        },
        {
          image:
            "https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRa7q8XhBB5inHO3kZa7CMM3NLEnAiVmgxTChTdxorZeVPQRRPu",
          name: "PRAVEEN"
        },
        {
          image:
            "https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRa7q8XhBB5inHO3kZa7CMM3NLEnAiVmgxTChTdxorZeVPQRRPu",
          name: "SOHAIL"
        },
        {
          image:
            "https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRa7q8XhBB5inHO3kZa7CMM3NLEnAiVmgxTChTdxorZeVPQRRPu",
          name: "NAVEEN"
        },
        {
          image:
            "https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRa7q8XhBB5inHO3kZa7CMM3NLEnAiVmgxTChTdxorZeVPQRRPu",
          name: "PRAVEEN"
        },
        {
          image:
            "https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRa7q8XhBB5inHO3kZa7CMM3NLEnAiVmgxTChTdxorZeVPQRRPu",
          name: "PRAVEEN"
        },
        {
          image:
            "https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRa7q8XhBB5inHO3kZa7CMM3NLEnAiVmgxTChTdxorZeVPQRRPu",
          name: "NAVEEN"
        },
        {
          image:
            "https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRa7q8XhBB5inHO3kZa7CMM3NLEnAiVmgxTChTdxorZeVPQRRPu",
          name: "SOHAIL"
        },
        {
          image:
            "https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRa7q8XhBB5inHO3kZa7CMM3NLEnAiVmgxTChTdxorZeVPQRRPu",
          name: "ANSH"
        }
      ]
    };
  },
  methods:{
    addFriend : function(){
      document.getElementById('myButton').value = "sentRequest";
      window.console.log('friend');
    }
  }
};
</script>
<style scoped>
button,
#myButton{
  width:100px;
  height:30px;
  background-color:#3b5998;
  color:white;
  border-radius:30px;
}
.image 
{
  height: 70px;
  width: 80px;
  border-radius: 50%;
  float:left;
}
.Friends {
  font-family: sans-serif;
  font-size: 20px;
  /* margin:auto;
  width:20%; */
}
.list{
  width:300px;
}
table {
  border : 1px solid black;
  width: 400px;
  padding:10px;
}
td{
    text-align:center;
    }
</style>