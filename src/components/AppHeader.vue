<template lang="">
    <header>
   <div class='logo'>
    <img src="../assets/img/dc-logo.png" alt="">
   </div>
   <nav>
    <ul>
        <li v-for="list in navList" >
         <a href="#">{{list.name}}</a>
        </li>
    </ul>
   </nav>
   
</header>
</template>


<script>
export default {
  name: "AppHeader",
  data() {
    return {
      navList: [
        {
          name: 'characters',
          active: false,
        },
        {
          name: 'comics',
          active: false,
        },
        {
          name: 'movies',
          active: false,
        },
        {
          name: 'tv',
          active: false,
        },
        {
          name: 'games',
          active: false,
        },
        {
          name: 'collectibles',
          active: false,
        },
        {
          name: 'videos',
          active: false,
        },
        {
          name: 'fans',
          active: false,
        },
        {
          name: 'news',
          active: false,
        },
        {
          name: 'shop',
          active: false,
        },
      ],
    };
  },
};
</script>


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

header{
    padding: 2rem 0;
    display: flex;
    justify-content: space-between;
    align-items:center;
    
}



ul{
  display: flex;
  list-style: none;
  
  li{
     margin-right: 1rem;
     text-transform: uppercase;
    
    a {
      text-decoration: none;
      color:rgb(65, 58, 61);
      
     }
     
     &:hover{
        border-bottom: 2px solid rgb(2, 130, 249);
        color: rgb(2, 130, 249);
     }
  }
}
</style>