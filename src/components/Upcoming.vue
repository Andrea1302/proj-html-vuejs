<template>
    <section id="upcoming" class="container">
        <h3 class="text-center">
            Upcoming Events
        </h3>
        <h5 class="text-center">
            MEET THE AUTHOR IN PERSON
        </h5>

        <!-- Cards  -->
        <div class="row">

            <!-- Card 1 -->
            <div class="col-lg-4">
                <img class="img_upcoming" src="../assets/event-05-800x479.jpg" alt="chicago">
                <h6 class="text-center">
                    Chicago Book Signing
                </h6>
                <p class="text-center">
                    Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a nulla.
                </p>
            </div>

            <!-- Card 2  -->
            <div class="col-lg-4">
                <img class="img_upcoming"  src="../assets/event-04-800x479.jpg" alt="Amanda">
                <h6 class="text-center">
                    Chicago Book Signing
                </h6>
                <p class="text-center">
                    Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Preaesent sapien massa, convallis a pellentesque nec, egestas
                </p>
            </div>


            <!-- Card 3  -->
            <div class="col-lg-4">
                <img class="img_upcoming"  src="../assets/event-07-800x479.jpg" alt="Book">
                <h6 class="text-center">
                    Chicago Book Signing
                </h6>
                <p class="text-center">
                    Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a. Mauris blandit aliquet elit, eget tincidunt nibh pulvinar a nulla.
                </p>
            </div>
        </div>
    </section>
</template>

<script>
export default {
  name: 'upcoming',
  props: {
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#upcoming{
    padding: 30px 0;
    h3{
        font-family: serif;
        font-weight: bold;
    }
    h5{
        font-size: .8rem;
        color: #e1aa40;
        margin-bottom: 30px;
    }
    .img_upcoming{
        width: 100%;
    }
    h6{
        margin: 20px 0 ;
    }
    p{
        color: #7c6e69;
        font-size: .8rem;
    }
}
</style>