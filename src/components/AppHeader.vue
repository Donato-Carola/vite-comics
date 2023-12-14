<template lang="">
    <header>
   <div class='logo'>
    
   </div>
   <nav>
    <ul>
        <li v-for="list in navList" >
         {{list.name}}
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

ul{
  list-style: none;
}
</style>