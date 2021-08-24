<template>
  <div class="hello">
    <li>
       <slot name="footer" :aa="title"> </slot>
    </li>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<style scoped>

</style>
