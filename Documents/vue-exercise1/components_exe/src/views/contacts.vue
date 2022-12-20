<template>
    <form>
        <label for="fullName">FullName</label>
        <input type="text" placeholder="FullName..." v-model="fullName">
        <label for="email">Email</label>
        <input type="email" placeholder="Email..." v-model="email">
        <label for="age">contact</label>
        <input type="number" placeholder="contact..." v-model="number">
        <input type="submit" id="submit" placeholder="Submit" v-on:click.prevent="submit">
    </form>
  </template>
  
  <script>
  // @ is an alias to /src
  import HelloWorld from '@/components/HelloWorld.vue'
  
  export default {
    name: 'HomeView',
    components: {
      HelloWorld
    }
  }
  submit(); {
                alert(`${this.fullName} with the email ${this.email} with number ${this.number}`)
            }

  </script>
  