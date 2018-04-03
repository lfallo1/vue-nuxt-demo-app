<template>
  <div>
    <h4>Users page {{formattedTitle}}</h4>
    <button @click="upper = !upper">Toggle Case</button>
    <div v-for="user in users">
      <nuxt-link :to="'/users/' + user">{{user}}</nuxt-link>
    </div>
    <div>
      <input type="text" v-model="userId" />
      <button @click="loadUser">Load User</button>
    </div>
    <hr>
    <br>
    <nuxt-child />
  </div>
</template>

<script>

  import NuxtChild from "../.nuxt/components/nuxt-child";

  export default {
    components: {NuxtChild},
    data(){
      return {
        upper: false,
        title: 'Page Title',
        users: ['lfallo1', 'bob123', 'john123', 'kate432'],
        userId: ''
      }
    },
    methods: {
      loadUser(){
        this.$router.push(`/users/${this.userId}`);
      }
    },
    computed:{
      formattedTitle(){
        if(this.title){
          return this.upper ? this.title.toUpperCase() : this.title
        }
        return '';
      }
    }
  }
</script>
