<template>
    <header class="container-fluid">

        <!-- layover sfondo  -->
        <div id="layover">
            <!-- navbar with logo e links -->
            <div class="row justify-content-between" id="navbar">
                <!-- logo  -->
                <img class="col-lg-2" :src="require(`../assets/${logopath}`)" alt="logo">

                <!-- links -->
                <nav class="col-lg-7">
                    <ul>
                        <li v-for="info,i in infoNav" :key="i">
                            <a href="#" :class="info.activeLink ? 'active' : '' " @click="activePage(info)">
                                {{info.link}}
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <i class="fas fa-shopping-cart"></i>
                            </a>
                        </li>
                    </ul> 
                </nav>
            </div>


            <!-- buy  -->
            <div id="info_shop">
                <div id="demos">
                    <button class="info_shop">
                        <i class="fas fa-archive"></i>
                        <div>
                            Demos
                        </div>
                    </button>
                </div>
                

                <button class="info_shop">
                    <span  id="onSale">
                        <sup>$</sup>
                        39
                    </span>
                    <div>
                        <span>
                            On Sale
                        </span> 
                    </div>
                </button>
            </div>
            <msJumbrotron />
        </div>
        
        
    </header>
</template>

<script>
// import jumbotron 
import msJumbrotron from '../components/MsJumbotron.vue';


export default {
  name: 'msHeader',
  components: {
    msJumbrotron,
  },
  props: {
    infoNav: Array,
    logopath : String,
  },
  data(){
     return {
    
     } 
  },
  methods : {
      activePage(object){
          if ( object.activeLink === false ) {
              object.activeLink = true 
          } else if (object.activeLink === true) {
              object.activeLink = false
          }
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    // active 
    .active{
        color: #f3b329;
        border-top: 4px solid #f3b329;
    }

    header{
        padding: 0;
        width: 100%;
        background-size: cover;
        background-position: top;
        background-image: url(../assets/hero-07-2x.jpg);
        #layover{
            background: rgb(0,0,0);
            background: linear-gradient(0deg, rgba(0,0,0,0.919765406162465) 0%, rgba(0,0,0,0.4861519607843137) 35%, rgba(0,0,0,0.2956757703081232) 100%);
            height: 100%;
        }
    }

    // info shop ù
    #info_shop{
        position: absolute;
        right : 10px;
        top : 80px
    }
    .info_shop{
        width: 40px;
        height: 40px;
        font-size: 8px;
        border-style: none;
        margin-bottom: 5px;
        border-radius: 5px;
        #onSale{
            font-size: 1.1rem;
            color: rgb(11, 179, 100);
        }
    }

    #navbar{
        padding: 0 50px;
    }

    nav{
        color: white;
        ul{
            display: flex;
            justify-content: space-between;
            li{
                list-style: none;
                a{
                    text-decoration: none;
                    color: white ;
                    font-weight: bold;
                    display: inline-block;
                    padding:30px 0
                }
            }
        }
    }
</style>