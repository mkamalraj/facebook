<template>
    <div class="Business">
        <div class="pages">
            <table border="1">
                <tr>
                    <th>BUSINESS PAGE</th>
                </tr>
                <tr v-for="(details,index) in pages" :key="index">
                    <td>{{details.name}}</td>
                </tr>
            </table>
        </div>
    </div>
</template>
<script>
export default {
    data(){
        return{
          pages:[
              {
                  name :"Coviam"
              },
              {
                  name :"Coviam"
              },
              {
                  name :"Coviam"
              },
              {
                  name :"Coviam"
              },
              {
                  name :"Coviam"
              },
              {
                  name :"Coviam"
              },
              ]
        }
    }
}
</script>
<style scoped>
.pages{
    width:40%;
    margin:auto;
}
table{ 
    width:500px;
    border-collapse:collapse;
}
th{
    text-align:center;
    background-color: #3b5998;
    color:white;
    font-size:20px;
}
tr{
    height:50px;
    text-align:center;
    /* padding-left:30px; */
}
</style>