<template>
  <div id="app">
    <!-- header  -->
      <msHeader 
        :infoNav ="this.navHeader"
        :logopath ="this.logo"
      />
    
    <!-- main  -->
    <msMain />

    <!-- Footer  -->
    <msFooter 
      :infoUsefulLinks ="this.links"
      :infoContact ="this.contact"
      :logopathFooter ="this.logo"
      :infoAboutMe ="this.aboutMe"
    />

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
    logo : "author-logo-round.png",
    // NavFooter
    links : ["Latest Books","Upcoming Events","Recent Articles","Business Enquires","Visit My Foundation"],
    contact : {
      address : "63 E. Studebaker Street Bolingbrook, IL 60440",
      phone : "(800) 000-0000",
      mobile : "(800) 000-0000",
      email : "info@your-company.com",
    },
    aboutMe : "Vivamus suscipit tortor eget felis porttitor volupat. Nulla quis lorem ut libero malesuada feugiat. Vivamus suscipit tortor eget felis porttitor volutpat"
        
      
    
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
  color: #2c3e50;
}

</style>
