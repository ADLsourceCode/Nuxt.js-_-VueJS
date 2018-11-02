<template>
<div class="post">
   
    <section class="all-posts">
      
    <PostPreview
    id="1"
    title="FIRST BLOG"
    contentPreview="Test content"
    thumbnail="https://fw-d7-freedomworks-org.s3.amazonaws.com/field/image/Tech.jpg"
    />

     <PostPreview
    id="2"
    title="SECOND BLOG"
    contentPreview="Test content"
    thumbnail="https://fw-d7-freedomworks-org.s3.amazonaws.com/field/image/Tech.jpg"
    />
    
  </section>
    </div>
</template>
 

<script>
import PostPreview from '~/components/PostPreview'
export default {
    components:{
        PostPreview
    }
}
</script>


 <style scoped>
 .post{
     display: flex;
     align-content: center;
     justify-content: center;
     margin-top: 20px;

 }

.all-posts {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}

 
 </style>
 