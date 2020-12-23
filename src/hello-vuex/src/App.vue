<template>
  <input type="button" v-on:click="ondecrement" value="-" />
  {{count}}
  <input type="button" v-on:click="onincrement" value="+" />
</template>

<script>
export default {
  name: 'App',
  computed:{
    count(){
      return this.$store.state.count
    },
  },
  methods:{
    onincrement(){
      this.$store.commit('increment')
    },
    ondecrement(){
      this.$store.commit('decrement')
    }
  }
}
</script>