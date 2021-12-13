<template>
  <div id="app">
    <!-- header  -->
      <msHeader 
        :infoNav ="this.navHeader"
      />
    
    <!-- main  -->
    <msMain />

    <!-- Footer  -->
    <msFooter />

  </div>
</template>

<script>
import msHeader from './components/MsHeader.vue';
import msFooter from './components/MsFooter.vue';
import msMain from './components/MsMain.vue';



export default {
  name: 'App',
  components: {
    msHeader,
    msFooter,
    msMain
  },
  data(){
  return {
    navHeader : 
      [
        {
          link : "Home",
          activeLink : true
        },
        {
          link : "About Me",
          activeLink : false
        },
        {
          link : "Testimonials",
          activeLink : false
        },
        {
          link : "My Blog",
          activeLink : false
        },
        {
          link : "Meetups",
          activeLink : false
        },
         {
          link : "Shop",
          activeLink : false
        },
         {
          link : "Contact Me",
          activeLink : false
        },
       ] ,
    logo : "",
    // NavFooter
    textDescription : "Vivamus suscipit tortor eget felis porttitor volupat. Nulla quis lorem ut libero malesuada feugiat. Vivamus suscipit tortor eget felis porttitor volutpat",
    links : ["Latest Books","Upcoming Events","Recent Articles","Business Enquires","Visit My Foundation"],
    Contact : {
      address : "63 E. Studebaker Street Bolingbrook, IL 60440",
      Phone : "(800) 000-0000",
      mobile : "(800) 000-0000",
      email : "info@your-company.com",
    }
        
      
    
  }
}
}

</script>

<style lang="scss">
*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

</style>
