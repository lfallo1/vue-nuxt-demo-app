<template>
  <div>
    <h4>Users page for user with id {{$route.params.id}}</h4>
    <div v-for="module in modules">
      <nuxt-link :to="'/users/' + $route.params.id + '/' + module">{{module}}</nuxt-link>
    </div>
  </div>
</template>

<script>

  export default {
    data(){
      return{
        modules: ['Account', 'Help', 'FAQ']
      }
    },
    validate(data){
      console.log('validating');
      console.log(data);
      return data.params.id.length < 10;
    }
  }
</script>
