<script setup>
import { ref } from "vue"
const Count = ref(0);
const addToCount = () =>{
  console.log("HELLO FORM ADD TO COUNT")
  Count.value = Count.value + 1;

}
const subtractFromCount = () =>{
  console.log("HELL FROM SUBTARC FROM COUNT")
  Count.value = Count.value - 1;
  
}

</script>
<!--script>
export default({
  data(){
    return{
      Count: 0
    
    }
  },
  method: {
    addToCount(){
      this.Count = this.Count + 1
    },
    subtractFromCount(){
      this.Count = this.Count - 1
    }
  }
})
</script-->
<template>
  <main>
    <div>
    <h4>The Current Counter....</h4>
    <h1>{{ Count }}</h1>

    <button @click="subtractFromCount()">-</button>
    <button @click="addToCount()">+</button>
  </div>
  </main>
 
</template>
<style scoped>
main{
  background-color: aliceblue;
  width: 100vw;
  height: 100vh;
  align-items: center;
  display: flex;
  justify-content: center;
}
div{
  text-align: center;
}</style>