<template>
    <section class="container" id="more_about">

        <!-- Title  -->
        <div class="text-center">
            <div class="col">
                <h2>
                    More About Damon Vaught
                </h2>
            </div>

            <!-- Description  -->
            <div class="row justify-content-center">
                <div class="col-lg-8">
                    <p>
                        Damon is a professor of psycology at the University of Toronto, a clinical psychologist and the autor of the multi-milion copy bestseller "The story of my life"
                    </p>
                </div>
            </div>

            <!-- Meet the Author  -->
            <button>
                Meet the Author
            </button>
        </div>

        <!-- sponsor -->
        <div class="row justify-content-center">
            <div class="col-lg-2">
                <img class="img_sponsor" src="../assets/ebay-logotan-2x-200x66.png" alt="ebay">
            </div>

             <div class="col-lg-2">
                <img class="img_sponsor" src="../assets/audible-logotan-2x-200x66.png" alt="audible">
            </div>

             <div class="col-lg-2">
                <img class="img_sponsor" src="../assets/bb-logotan-2x-200x66.png" alt="barnes_noble">
            </div>

             <div class="col-lg-2">
                <img class="img_sponsor" src="../assets/kindlefire-logotan-2x-200x66.png" alt="kindle_fire">
            </div>

        </div>
    </section>
</template>

<script>
export default {
  name: 'moreAbout',
  props: {

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Shalimar&display=swap');
#more_about{
    padding: 50px 0 ;
    button{
        padding: 5px 10px;
        border-style: none;
        border-radius: 2px;
        color: white;
        background-color:#3da698 ;
        font-size: .7rem;
        font-weight: bold;
        margin-bottom: 100px;
    }
    // img 
    .img_sponsor{
        width: 70%;
    }
}
// Titolo 
 h2{
    font-family: Shalimar;
    color: #e1aa40;
    font-weight: bold;
    font-size: 50px;
}

// hover
#more_about{
    button:hover{
        background-color: #3e9c90;
    }
}
</style>