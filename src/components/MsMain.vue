<template>
    <main>
        <moreAbout/>
        <newAudioBook/>
    </main>
</template>

<script>
import moreAbout from "../components/MoreAboutDamon.vue"
import newAudioBook from "../components/NewAudiobook.vue"
export default {
  name: 'msMain',
  components : {
    moreAbout,
    newAudioBook
  },
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>