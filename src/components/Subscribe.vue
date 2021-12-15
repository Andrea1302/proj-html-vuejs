<template>
    <section id="subscribe">

        <div id="container_subscribe">
            <!-- Title  -->

            <h3 class="col-lg-6 text-center">
                Subscribe To My Newsletter
            </h3>
        
            <!-- Subtitle  -->
            <h4 class="col text-center">
                BE NOTIFIED ABOUT BOOK SIGNING TOUR DATES
            </h4>

            <!-- input email e invio  -->
            <div id="input_mail">
                <input class="col-lg-6" type="text" placeholder="Insert your email...*" name="" id="">
                <button class="col-lg-5">
                    Subscribe
                </button>
            </div>

            <p class="text-center">
                Donec fringilla nunc eu turpis dignissim, at eusimod sapien tincidunt
            </p>
        </div>
        
        
    </section>
</template>

<script>
export default {
  name: 'subscribe',
  props: {

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#subscribe{
    min-height: 239px;
    background-image: url(../assets/banner-2.jpg);
    background-size: cover;
    background-position: top;
    display: flex;
    align-items: center;
    h3{
        color: white;
        font-family: serif;
        font-weight:bold;
        font-size: 1.4rem;
    }
    h4{
        font-size: .8rem;
        color: #f3b329;
        font-weight: bold;
    }
    #container_subscribe{
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        width: 27%;
        margin: 0 auto;
        #input_mail{
            width: 100%;
            display: flex;
            justify-content: space-between;
            margin: 10px 0;
            input{
                padding: 6px 5px;
                border-radius: 5px;
                font-size: .7rem;
            }
            button{
                border-radius: 5px;
                border-style: none;
                color: white;
                background-color: #3da698;
                font-weight: bold;
                font-size: .7rem;
            }
        }
        p{
            color: #7c6e60;
            font-size: .7rem;
        }
    }
}
</style>