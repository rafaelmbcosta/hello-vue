<template>
  <div>
    <h1> Server status: {{ status }}</h1>
    <hr/>
    <button @click="changeStatus">Change Server Status</button>
  </div>
</template>

<script>
  export default{
    data: function(){
      return{
        status: 'Critical'
      }
    },
    methods: {
      changeStatus(){
        this.status = 'Normal';
      }
    }
  }
</script>
