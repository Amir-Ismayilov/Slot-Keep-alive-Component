<template>
  <div>
    <h1>Yeni Anı Componenti....</h1>
    <p>Shows functionality keep-alive</p>
    <button @click="counter++">PLUS +</button>
    <p> {{ counter }}</p>
    <p>check console</p>
  </div>
</template>
<script>
  export default {
    data : function(){
      return {
        counter : 0
      }
    },
    destroyed(){
      console.log("Destroyed!!!");
    },
    activated(){
      console.log("Activated!!!")
    },
    deactivated(){
      console.log("DeActivated!!!")
    }
  }
</script>
