<template>
    <header>
        <nav>
            qui inserirò la navbar 
        </nav>
    </header>
</template>

<script>
export default {
  name: 'msHeader',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    // debug
    header{
        height: 300px;
        background-color: black;
    }
    nav{
        height: 100px;
        background-color: rgba(199, 199, 199, 0.144);
        color: white;
    }
</style>