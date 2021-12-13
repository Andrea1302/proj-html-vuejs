<template>
    <footer>
        Qui ci sarà il footer
    </footer>
</template>

<script>
export default {
  name: 'msFooter',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    // debug
    footer{
        height: 300px;
        background-color: grey;
    }
</style>