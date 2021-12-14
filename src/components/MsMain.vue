<template>
    <main>
        <moreAbout/>
        <newAudioBook/>
        <crities/>
        <upcoming />
        <subscribe/>
    </main>
</template>

<script>
import moreAbout from "../components/MoreAboutDamon.vue";
import newAudioBook from "../components/NewAudiobook.vue";
import crities from "../components/Crities.vue";
import upcoming from "../components/Upcoming.vue";
import subscribe from "../components/Subscribe.vue"

export default {
  name: 'msMain',
  components : {
    moreAbout,
    newAudioBook,
    crities,
    upcoming,
    subscribe
  },
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>