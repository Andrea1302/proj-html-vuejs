<template>
    <header class="container">
        <div class="row justify-content-around" id="navbar">
            <img class="col-lg-2" src="../assets/author-logo-round.png" alt="logo">
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
        color: orange;
        border-top: 4px solid orange;
    }

    header{
        width: 100%;
        min-height: 550px;
        background-size: cover;
        background-position: top;
        background-image: url(../assets/hero-07-2x.jpg);
    }
    nav{
        height: 100px;
        background-color: rgba(102, 22, 22, 0.144);
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