<template>
  <button class="btn">{{ title }}</button>
</template>

<script>
  export default {
    name: "SimpleButton"
  }

  Vue.component('simple_button', {
    template: '#btn-template',
    props: {
      title: String,
      btnClass: String
    }
  })

  new Vue({el: '#app'})
</script>

<style scoped>
  .btn {
    width: 150px;
    height: 40px;
    border-radius: 10px;
    font-size: 20px;
    color: white;
    border: 1px solid #64bab7;
    box-shadow: 4px 4px 7px #8bcbc9;
  }

  .blueBtn {
    background: linear-gradient(to top, #087d78 0%,  #64BAB7 100%);
  }

  .redBtn {
    background: linear-gradient(to top, #A51F29 0%,  #FF616C 100%);
  }
</style>