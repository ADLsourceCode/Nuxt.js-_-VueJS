<template>
<div class="new-post-form" @submit.prevent="OnSave"> 
<AdminForm/>
          
</div>

</template>



<script>
import AdminForm from '@/components/admin-post-form'


export default {
    components:{
        AdminForm
    },
    methods:{
        
    }
}
</script>


<style scoped>

</style>
