<template>
  <router-link :to='page' tag="button">{{buttonText}}</router-link>
</template>

<script>
export default {
  name:'navbarButton',
  props:['buttonText', 'page'],
  methods:{
    loadPage(_page){
      console.log(_page);
    }
  },
}
</script>

<style scoped>
button{
  margin-right:50px;
  padding:15px;
  border:none;
  background-color:transparent;
  font-size:16px;
  font-weight: 400;
  color:yellow;
}

@media(max-width:480px){
  button{
    margin:0;
    padding:20px;
    width:100%;
    text-align: left;
    border-bottom: 1px solid #9fa5a9;
    text-decoration: none;
  }
}
</style>
