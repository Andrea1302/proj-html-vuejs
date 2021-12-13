<template>
    <header class="container">

        <!-- layover sfondo  -->
        <div id="layover">
            <!-- navbar with logo e links -->
            <div class="row justify-content-around" id="navbar">
                <!-- logo  -->
                <img class="col-lg-2" src="../assets/author-logo-round.png" alt="logo">
                <!-- links -->
                <nav class="col-lg-6">
                    <ul>
                        <li v-for="info,i in infoNav" :key="i">
                            <a href="#" :class="info.activeLink ? 'active' : '' ">
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
        </div>
        
        
    </header>
</template>

<script>
export default {
  name: 'msHeader',
  props: {
    infoNav: Array
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
        height: 550px;
        background-size: cover;
        background-position: top;
        background-image: url(../assets/hero-07-2x.jpg);
        #layover{
            background: rgb(0,0,0);
            background: linear-gradient(0deg, rgba(0,0,0,0.919765406162465) 0%, rgba(0,0,0,0.4861519607843137) 35%, rgba(0,0,0,0.2956757703081232) 100%);
            height: 100%;
        }
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