<template>
    <div class="ImageUpload">
        <input type="file" @change="onFileSelected">
        <button v-bind:click="onUpload">Upload</button>
    </div>
</template>
<script>
import axios from 'axios'
export default {
    data(){
        return{
           SelectedFile :null
        }
    },
    methods:{
        onFileSelected(event){
         window.console.log(event);
         this.SelectedFile = event.target.files[0]
        },
        onUpload(){
        const fd  = new FormData();
        fd.append('image',this.SelectedFile,this.SelectedFile.name) 
        axios.post('https://console.firebase.google.com/project/vue-upload-fa5b8/storage/vue-upload-fa5b8.appspot.com/files~2F')
        .then(res => {
         window.console.log(res);
        })
        }
    }
}
</script>