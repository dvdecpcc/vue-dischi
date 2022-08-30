<template>
  <div class="myDisc text-center p-3">
    <div class="p-3">
        <img class="img-fluid mb-2" :src="disc.poster" alt="disc.name">
        <p class="card-title fw-bold text-uppercase title">{{disc.title}}</p>
        <p class="card-subtitle">{{disc.author}}</p>
        <p class="card-subtitle">{{disc.year}}</p>
    </div>
  </div>
</template>

<script>
export default {
    name: 'MyDisc',
    props: {
        disc: Object,
    },
}
</script>

<style scoped lang="scss">
    .myDisc{
        flex-basis: calc(100%/5);

        
        div{
            height: 100%;
            background-color: rgb(46, 58, 70);

            .title{color: white;}
        }
    }
</style>