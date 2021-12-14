<template>
    <main>
        <moreAbout/>
    </main>
</template>

<script>
import moreAbout from "../components/MoreAboutDamon.vue"
export default {
  name: 'msMain',
  components : {
    moreAbout
  },
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
// debug
    main{
        background-color: white;
    }
</style>