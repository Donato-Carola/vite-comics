<template lang="">
  <footer>

    <section class='logoSection'>

      
   </section>
    <section class='firstSection'>
      <div>
        <h2>dc comics</h2>
        <ul>
          <li>characters</li>
          <li>characters</li>
          <li>characters</li>
          <li>characters</li>
          <li>characters</li>
          <li>characters</li>
          <li>characters</li>
        </ul>

        <h2>shop</h2>
        <ul>
          <li>shopdc</li>
          <li>shopdc</li>
        </ul>
      </div>

      <div>
        <h2>dc</h2>
        <ul>
          <li>characters</li>
          <li>characters</li>
          <li>characters</li>
          <li>characters</li>
          <li>characters</li>
          <li>characters</li>
          <li>characters</li>
          <li>characters</li>
          <li>characters</li>
          <li>characters</li>
          <li>characters</li>
        </ul>
      </div>
      
      <div>
        <h2>sites</h2>
         <ul>
            <li>characters</li>
            <li>characters</li>
            <li>characters</li>
            <li>characters</li>
            <li>characters</li>
         </ul>
      </div>
       

   <div class='logo'>
    <img src="../assets/img/dc-logo-bg.png" alt="">
   </div>

    </section>
  </footer>

  <div class='underFooter'>
    <section>
      <div>
        <button>
            <span>sign-up now</span>
        </button>
      </div>
      <div class='iconSocial'>
         <span>follow us</span>
         <img src="../assets/img/footer-facebook.png" alt="">
         <img src="../assets/img/footer-facebook.png" alt="">
         <img src="../assets/img/footer-facebook.png" alt="">
         <img src="../assets/img/footer-facebook.png" alt="">
         <img src="../assets/img/footer-facebook.png" alt="">
      </div>
      </section>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

footer {
 
  background-repeat: no-repeat;  
  background-image: url(../assets/img/footer-bg.jpg);
  background-size: cover;
}

section.logoSection{
  height: 200px;
  background-color: rgb(2, 130, 249);
}


section.firstSection {
    position: relative;
  width: 1200px;
  margin: 0 auto;
  display: flex;
  padding: 3rem 0;

  h2 {
    text-transform: uppercase;
    padding-top: 1.5rem;
    padding-right: 4rem;
    color: white;
  }

  ul {
    list-style: none;
    color: rgb(149, 149, 149);

    li {
      padding-top: 0.5rem;
    }
  }

  div.logo{
  
    position: absolute;
    top: -20px;
    right: 0;
  }
}

div.underFooter{
  position: absolute;
    width: 100%;
  z-index: 3;
 background-color: rgb(48, 48, 48);

 
 section{
    width: 1200px;
  margin: 0 auto;
  padding:2rem 0 ;
  display: flex;
  justify-content: space-between;
  align-items: center;

  div.iconSocial{
    display: flex;
    align-items: center;
    img{
        padding: 0 1rem;
    }
    
  }
 }
 

       
   
}

button{
padding: 1rem;
background-color: rgb(48, 48, 48);
color: white;
border: 1px solid rgb(2, 130, 249);

    
}

span{
       text-transform: uppercase;
    }


</style>
