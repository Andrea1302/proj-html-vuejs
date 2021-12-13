<template>
    <footer>
        <div class="row justify-content-center">
            <div class="col-lg-3">
              <ul> 
                ABOUT ME
                <li>
                  Vivamus suscipit tortor eget felis porttitor volupat. Nulla quis lorem ut libero malesuada feugiat. Vivamus suscipit tortor eget felis porttitor volutpat
                </li>
              </ul>
            </div>
            <div class="col-lg-3">
              <ul>
                USEFUL LINKS
                <li v-for="link,i in infoUsefulLinks" :key="i">
                  <a href="#">
                    <i class="fas fa-angle-right arrow_right"></i> {{link}}
                  </a>
                </li>
              </ul>
            </div>
              
            <div class="col-lg-3">
              <ul>
                CONTACT INFO 
                <li>
                  <a href="#">
                    {{infoContact.address}}
                  </a>
                </li>

                <li>
                  <a href="#">
                    Phone:{{infoContact.phone}}
                  </a>
                </li>

                <li>
                  <a href="#">
                    Mobile:{{infoContact.mobile}}
                  </a>
                </li>

                <li>
                  <a href="#">
                    Email:{{infoContact.email}}
                  </a>
                </li>
                
                <!-- social  -->
                <li>
                  <!-- facebook -->
                  <a href="#">
                    <i class="fab fa-facebook-f social"></i>
                  </a>

                  <!-- twitter  -->
                  <a href="#">
                    <i class="fab fa-twitter social"></i>
                  </a>

                  <!-- Instagram  -->
                  <a href="#">
                    <i class="fab fa-instagram social"></i>
                  </a>

                  <!-- Linkedin -->
                  <a href="#">
                    <i class="fab fa-linkedin-in social"></i>
                  </a>
                  
                  <!-- Youtube -->
                  <a href="#">
                    <i class="fab fa-youtube social"></i>
                  </a>
                </li>
              </ul>
            </div>
        </div>
        <div id="copyright" class="text-center">
          &#169; Copyright 2012 - 2020 | Avada Theme by <a href="#">Theme Fusion</a> | All Rights Reserved | Powered by <a href="#">WordPress</a>
        </div>
    </footer>
    
</template>

<script>
export default {
  name: 'msFooter',
  props: {
    infoUsefulLinks : Array,
    infoContact : Object
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    // debug
    footer{
        
        padding: 50px;
        background-image: url(../assets/footer-3.jpg);
        background-size: cover;
        color: white;
        ul{
          font-weight: bold;
        } li {
          font-size: .7rem;
          margin: 12px 0;
          list-style: none;
          padding: 0;
          .arrow_right{
            margin-right: 10px;
          }
          .social{
            margin-right: 20px;
            font-size: 15px;
          }
          a{
            text-decoration: none;
            color: white;
          }
        }
        #copyright{
          font-size: .7rem;
          color:#96a4a3;
          margin-top: 20px;
          a{
            color: white;
            text-decoration: none;
            font-weight: bold;
          }
        }
    }
</style>