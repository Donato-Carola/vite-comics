<template>
  <main>
    <img src="../assets/img/jumbotron.jpg" alt="" />

    <section>
      <div class="series">
        <span>cureent series</span>
      </div>
      <div>
        <ListHero
          v-for="hero in heroList"
          :imageSrc="hero.thumb"
          :title="hero.series"
        />
      </div>
      <div class="button">
        <button>load more</button>
      </div>
    </section>
  </main>
</template>

<script>
import ListHero from "./ListHero.vue";

export default {
  name: "AppMain",
  data() {
    return {
      heroList: [
        {
          thumb: "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book",
        },
        {
          thumb:
            "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book",
        },
        {
          thumb:
            "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel",
        },
        {
          thumb: "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book",
        },
        {
          thumb:
            "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
          price: "$3.99",
          series: "Batman",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel",
        },
      ],
    };
  },
  components: {
    ListHero,
  },
};
</script>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

main {
  background-color: rgb(28, 28, 28);
  position: relative;

  img {
    width: 100%;
    background-repeat: no-repeat;
    background-size: cover;
  }
}

section {
  padding: 2rem 0;
  background-color: rgb(31, 31, 31);
  position: absolute;
  bottom: 0;
  width: 100%;

  div {
    display: flex;
    flex-wrap: wrap;
    width: 1200px;
    margin: 0 auto;
  }
}

div.series {
  position: absolute;
  bottom: 95%;
  left: 150px;
  width: 12%;
  background-color: rgb(2, 130, 249);
  padding: 1rem 1.5rem;
  color: white;
  text-transform: uppercase;
}

div.button{
  justify-content: center;
  
  
  
  button {
    padding: 0.5rem 2.5rem;
    background-color: rgb(2, 130, 249);
    border: 0;
    color: white;

  text-transform: uppercase; 
   
}
}

</style>
