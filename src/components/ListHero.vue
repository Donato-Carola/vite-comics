<template >

    
    <article>
        <img :src="imageSrc" alt="">
        <div>
            {{ title }}
        </div>
    </article>
            

</template>


<script>
export default {
    name:'ListHero',
    props: {
        imageSrc: String,
        title: String,
    }
}
</script>




<style lang="scss" >

 article{
    
    width: calc(100% / 6 - 1rem);
    margin-left: 0.5rem;
    margin-right: 0.5rem;
    margin-bottom: 0.5rem;
    color: white;
    
    img{
        width: 100%;
        height: 200px;
        background-size: cover;
        
       
    }
   
 }


    
</style>