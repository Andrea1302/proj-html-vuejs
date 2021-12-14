<template>
    <section class="container" id="crities">
        
        <div class="row">
            <!-- title  -->
            <div class="col">
                <h5  id="title">
                     What The Crities Say
                </h5>
                <div id="subtitle">
                    TESTIMONIALS FROM AROUND THE WORLD
                </div>
            </div>
            <!-- Read  -->
            <div id="button">
                <button>
                    Read All Testimonials
                </button>
            </div>
            
        </div>

        <!-- Card and description  -->

        <div class="row justify-content-around">
            <div class="col-lg-6" id="card_testimoniance">
                <h3>
                    Best Author Of His Generation
                </h3>

                <hr>

                <h6>
                    This book will change your perspective on life
                </h6>

                <p>
                    Donec fringilla nunc eu turpis dignissim, at eusimod sapien tincidunt. Maecenas eleifend congue cursus. In vitae enim quis sem pharetra. Curabitur arcu erat, accumsan id imperdiet et, porttitor at sem.
                </p>

                <p>
                    Donec rutrum congue leo eget malesuada. Vivamus suscipit tortor eget felis porttitor voluptat. Nulla quis Lorem ut liber. Proin eget tortor risus. Praesent sapien massa, convallis a pallentesque nec, egestas non nisi. Donec rutrum congue leo eget malesuada.
                </p>

                <cite>
                    <img class="logo" src="https://greenlee.iastate.edu/wp-content/uploads/sites/186/2019/10/t_logo_2048_black.png" alt="ny_times_logo">
                    Justine Killpatrick, <span>The New York Times</span>
                </cite>
            </div>

            <!-- other testimoniance  -->
            <div class="col-lg-5">
                <div class="other_mini_card">
                     <h5 class="text-center">
                        A True Masterpiece, Bravo!
                    </h5>
                    <p class="text-center">
                        Nulla quis lorem ut libero malesuada feugiat.Vivamous magna justo, lacinia eget consectur sed, convallis at tellus. Vivamus suscipt tortor eget felis porttitor voluptat. Nulla quis Lorem ut libero malesuada feug at.
                    </p>
                </div>
                <img class="logo_mini_card" src="https://img.favpng.com/15/4/19/the-guardian-guardian-media-group-theguardian-com-news-journalism-png-favpng-PMAjkdA8PkC7NrdUr4kXAskeK.jpg" alt="logo_the_guardian">
                <cite class="citazione">Gerarld Hendley, <span class="journal"> The Guardian </span> </cite>
                <div class="other_mini_card">
                     <h5 class="text-center">
                        A Unique View On The World
                    </h5>
                    <p class="text-center">
                        Donec sollicitudin molestie malesuada. Curabitur arcu erat, accumsan id imperdiet et, porttitor at sem. Vestibulum ac diam sit amet quam vehicula elementum sed sit amet dui. Nulla qui lorem ut libero malesuada feugiat. Vestibulum ac diam sit amet
                    </p>
                </div>
                <img class="logo_mini_card_2" src="https://taskful.com/_next/static/images/theglobeandmail-7817187f4cd5c42ae4d339ad5f4709b1.png" alt="logo_the_globe_mail">
                <cite class="citazione">Mary Maxey,<span class="journal"> The Globe And Mail </span> </cite>
               
            </div>
        </div>
    </section>
</template>

<script>
export default {
  name: 'crities',
  props: {
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#crities{
    padding: 30px 0;
    position: relative;
    #title{
        font-weight: bold;
        font-family: serif;
    }
    #subtitle{
        font-size: .7rem;
        color: #3da698;
        margin-bottom: 20px;
    }        
    button{
        position: absolute;
        top: 40px;
        right: 0;
        color: white;
        font-weight: bold;
        padding: 5px 20px;
        border-radius: 2px;
        background-color: #e1aa40;
        border-style: none;
        font-size: .7rem;
    }

    // card 
    #card_testimoniance{
        padding: 60px;
        background-image: url(../assets/testimonial2-2x.jpg);
        background-size: cover;
        background-position: center;
        color: white;
        border-bottom-right-radius: 10%;
        h3{
            font-weight: bold;
            font-family: serif;
        }
        h6, p {
            font-weight: bold;
        }
        p{
            font-size: .8rem;
        }
    }
    .logo{
        width: 8%;
    }
    cite{
        font-weight: bold;
        span{
            color:#3da698 ;
        }
    }

    // minicard
    .logo_mini_card{
        width: 13%;
        margin-right: 15px;
    }
    .logo_mini_card_2{
        width: 9%;
        margin-right: 15px;
        margin-left: 9px;
    }
    .other_mini_card{
        width: 80%;
        margin: 30px auto;
        h5{
            font-weight: bold;
            font-family: serif;
        }
        p{
            color: #7c6e60;
            font-size: .8rem;
        }
    }
    .citazione{
        font-weight: bold;
        font-size: .7rem;
        color: #7c6e60;
    }
    .journal{
        color: black;
        font-weight: normal;
    }
}
</style>