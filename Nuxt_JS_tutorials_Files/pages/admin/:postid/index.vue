<template>
    <AdminForm :postId="loadedPost" />
</template>


<script>
import AdminForm from '~/components/admin-post-form'
export default {
    components:{
        AdminForm
    },
    data(){
        return {
            loadedPost:{
                author:'TEST',
                title:'TITLE 1',
                content:'TEsT CONTENT',
                thumbnailLink:"https://fw-d7-freedomworks-org.s3.amazonaws.com/field/image/Tech.jpg"
            }
        }
    }
}
</script>

<style scoped>

</style>
