<template>
  <div class="hello">
    <li>
        --{{$attrs.color}}
        <slot name="app" :slotName="slotName"></slot>
        <button @click="changeSlot">改变slot</button>
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
