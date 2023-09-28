<script>
    export default{
      data(){
        return{
          arr:[],
          input:'',
        }
      },
      methods:{
        push(){
          this.arr.push(this.input)
          this.input=''
        }
      }
    }
</script>

<template>
  <h1>Lista spesa</h1>
  <input type="text" v-model="input">
  <button @click="push">Invia</button>
  <ul>
    <li v-for="element in arr" :key="element" >{{ element }}</li>
  </ul>
</template>

<style scoped>

</style>
