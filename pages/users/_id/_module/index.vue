<template>
  <div>
    <h4>id {{ $route.params.id }}</h4>
    <h4 v-if="$route.params.module">module: {{$route.params.module}} </h4>
  </div>
</template>

<script>

  export default {
    data(){
      return {}
    },
    created(){

    }
  }
</script>
