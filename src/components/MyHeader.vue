<template>
  <div class="myHeader d-flex align-items-center p-2">
    <img src="@/assets/img/logo-small.svg" alt="spotify logo">
  </div>
</template>

<script>
export default {
    name: 'MyHeader',
}
</script>

<style scoped lang="scss">
    .myHeader{
        background-color: rgb(46, 58, 70);
    }
    img{
      height: 30px;  
    }
    
</style>