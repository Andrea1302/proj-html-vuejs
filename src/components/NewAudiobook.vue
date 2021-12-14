<template>
    <section id="new_audio_book">
        <div class="container">
            <div class="row justify-content-center" id="row_audio_book">
                <div class="col-lg-4">
                    <img src="../assets/audible-app-2x-200x209.png" alt="audiobook">
                </div>

                 <div class="col-lg-4" id="description">
                     <h3>
                         New Audiobook
                     </h3>

                     <h4>
                         NO TIME TO READ? NO PROBLEM, LISTEN TO IT
                     </h4>

                     <p>
                         Donec fringilla runc eu turpis dignissim at euismod sapien tincidunt. Maecenas eleifend congue cursus.
                     </p>
                    <div class="row justify-content-center">
                        <div class="col">
                            <img class="img_sponsor" src="../assets/audible-logo.png" alt="audible">
                        </div>
                        <div class="col">
                            <img class="img_sponsor" src="../assets/bn-logo-tall.png" alt="barnes_noble">
                        </div>
                        <div class="col">
                            <img class="img_sponsor" src="../assets/kindle-logo-tall.png" alt="kindle_fire">
                        </div>
                    </div>
                    

                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
  name: 'newAudioBook',
  props: {

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#new_audio_book{
    background-image: url(../assets/banner.jpg);
    background-size: cover;
}
#row_audio_book{
    padding-top: 30px;
}
#description{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    h3{
        font-size: 1.3rem;
        color: white;
        font-weight: bold;
        font-family: serif;
    }
    h4{
        font-size: .7rem;
        font-weight: bold;
        color: #e1aa40;
    }
    p{
        font-size: .6rem;
        color:#96a4a3;
        width: 80%
    };
}
.img_sponsor{
    max-width: 90%;
}
</style>