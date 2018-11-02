
<template>
<div>
<AppControlInput v-model="editedPost.author">Author Name</AppControlInput>
        
<AppControlInput v-model="editedPost.title">Title</AppControlInput>
        
<AppControlInput v-model="editedPost.thumbnailLink">Thumbnail Link</AppControlInput>
        
<AppControlInput
          control-type="textarea"
          v-model="editedPost.content">Content</AppControlInput>
        
<AppButton type="submit">Save</AppButton>
        
<AppButton
          type="button"
          style="margin-left: 10px"
          btn-style="cancel"
          @click="onCancel">Cancel</AppButton>    

</div>
</template>


<script>
import AppControlInput from '@/components/AppControlInput'
import AppButton from '@/components/AppButton'

export default {
    props:{
        postId:{
            type:Object,
            required:false
        }
    },
    components:{
        AppControlInput,
        AppButton
    },
    data(){
        return{
editedPost: this.postId ? {...this.postId}:{
    title:'',
    author:'',
    thumbnailLink:'',
    content:''
}
}
    },
    methods:{
        onCancel(){
              this.$router.push('/admin')  
        },
        OnSave(){
            console.log(this.editedPost)
        }
    }
}

</script>
