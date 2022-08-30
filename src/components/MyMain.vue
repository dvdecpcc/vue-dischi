<template>
  <div class="container">
    <div class="d-flex flex-wrap">
        <MyDisc
            v-for="(discItem, index) in discs"
            :key='index'
            :disc='discItem'
        />
    </div>
  </div>
</template>

<script>
import axios from 'axios';
import MyDisc from './MyDisc';

export default {
    name: 'MyMain',
    components: {
        MyDisc,
    },
    data() {
        return {
            discs: [],
        };
    },
    created() {
        axios
        .get("https://flynn.boolean.careers/exercises/api/array/music")
        .then((res) => {
            this.discs=res.data.response;
        })
    }
}
</script>

<style scoped lang="scss">

</style>