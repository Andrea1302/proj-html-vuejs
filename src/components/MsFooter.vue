<template>
    <footer>
        <div class="row justify-content-center">
            <div class="col-lg-3">
              <h6>
                ABOUT ME
              </h6>
              <p>
                Vivamus suscipit tortor eget felis porttitor volupat. Nulla quis lorem ut libero malesuada feugiat. Vivamus suscipit tortor eget felis porttitor volutpat
              </p>
            </div>
            <div class="col-lg-3">
              <h6>
                USEFUL LINKS
              </h6>
              <ul>
                <li v-for="link,i in infoUsefulLinks" :key="i">
                  <a href="#">
                    {{link}}
                  </a>
                </li>
              </ul>
            </div>
              
            <div class="col-lg-3">
              <h6>
                CONTACT INFO 
              </h6>
              <ul>
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
                
              </ul>
            </div>
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
        // debug
        height: 500px;

        padding: 50px;
        background-image: url(../assets/footer-3.jpg);
        background-size: cover;
        color: white;
        ul{
          font-weight: bold;
        } li {
          list-style: none;
        }
    }
</style>