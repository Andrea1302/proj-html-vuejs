<template>
    <section id="more_info" class="container">
        <h3 class="text-center">
            Dig A Little Deeper Into Damon Vaugh
        </h3>
        <h6 class="text-center">
            FIND OUT MORE ABOUT THE AUTHOR HIMSELF
        </h6>

        <!-- card  -->
        <div class="row justify-content-center">

            <!-- card 1  -->
            <div class="col-lg-3 px-0 card" id="about_me_card">
                <div class="layover text-center">
                    <h4>
                        About Me
                    </h4>
                    <div class="hr">

                    </div>
                    <h5>
                        Vestibulum ante ipsum primis
                    </h5>
                </div>
            </div>
            <!-- card2 -->
            <div class="col-lg-3 px-0 card" id="my_latest_book_card">
                <div class="layover text-center">
                     <h4>
                        My Latest Book
                    </h4>

                    <div class="hr">

                    </div>
                    <h5>
                        Vestibulum ante ipsum primis
                    </h5>
                </div>
            </div>
            <!-- card3 -->
            <div class="col-lg-3 px-0 card" id="book_signing_card">
                <div class="layover text-center">
                     <h4>
                        Book Signing
                    </h4>
                    <div class="hr">

                    </div>
                    <h5>
                        Vestibulum ante ipsum primis
                    </h5>
                </div>
            </div>

        </div>
    </section>
</template>

<script>
export default {
  name: 'moreInfo',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#more_info{
    padding: 60px 0 ;
    h3{
        font-family: serif;
        font-weight: bold;
    }
    h6{
        margin-bottom: 30px;
        font-size: .7rem;
        color:#3da698 ;
    }
    .layover{
        padding: 20px 0;
        display: flex;
        flex-direction: column;
        justify-content: flex-end;
        border-bottom-right-radius: 30px;
        width: 100%;
        height: 100%;
        background: rgb(0,0,0);
        background: linear-gradient(0deg, rgba(0,0,0,0.5626225490196079) 0%,  rgba(0,0,0,0.450577731092437) 39%, rgba(0,0,0,0.1861519607843137) 78%, rgba(0,0,0,0.0956757703081232) 100%);
        .hr{
            width: 20%;
            margin: 10px auto;
            border-bottom: 2px solid rgba(255, 255, 255, 0.199)
        }
        h4{
            color: white;
            margin-bottom: 0;
        }
        h5{
            color: #e1aa40;
            font-size: .9rem;
        }
    }
    #about_me_card{
        background-image: url(../assets/box-1.jpg);
        background-size: cover;
        background-position: center; 
        background-repeat: no-repeat;
    }
    #my_latest_book_card{
        background-image: url(../assets/box-4.jpg);
        background-size: cover;
        background-position: center; 
        background-repeat: no-repeat;

    }
    #book_signing_card{
        background-image: url(../assets/box-3.jpg);
        background-size: cover;
        background-position: center; 
        background-repeat: no-repeat;

    }
    .card{
        height: 350px;
        border-bottom-right-radius: 30px;
        margin: 0 10px;
    }
}
</style>

