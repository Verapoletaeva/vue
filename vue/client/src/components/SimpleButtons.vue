<template id="btn-template">
  <div class="button">{{ title }}</div>
</template>

<script>

  Vue.component('simple_button', {
    props: ['title'],
    template: '<button class="btn">{{ title }}</button>'
  })

  new Vue({el: '#button'})
</script>

<style>
  button {
    width: 150px;
    height: 40px;
    font-size: 14px;
    border-radius: 10px;
  }
</style>