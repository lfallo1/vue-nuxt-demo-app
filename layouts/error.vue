<template>
  <div>
    <h3>You've cased a disaster</h3>
    <h2>{{error.statusCode}} | {{error.message}}</h2>
    <nuxt-link to="/">Home</nuxt-link>
  </div>
</template>

<script>

  export default{
    props: ['error'],
    created(){
      console.log(this.error);
    }
  }

</script>
