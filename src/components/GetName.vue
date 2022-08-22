<template>
  <div class="get-name" @click="getNameFromServer">
  {{myName}}
  </div>
</template>

<script>

export default {
    name: "getName",
    data(){
      return {
        myName: '初始的名字'
      }
    },
    methods:{
      getNameFromServer() {
        const request = new XMLHttpRequest()
        request.open('get', 'localhost:3000')
        request.send()
        request.onreadystatechange = () => {
          if (request.readyState === 4) {
            console.log(request.responseText);
          }
        }
      }
    }
}
</script>

<style>
.get-name {
  width: 100px;
  height: 40px;
  background: #999;
  border: solid 2px lightgreen;
  border-radius: 20%;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
