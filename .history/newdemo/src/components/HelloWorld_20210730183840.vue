<template>
  <div class="hello">
    <li>
        --{{$attrs.color}}
        <slot name="app" :data="data"></slot>
        <button @click="changeSlot">改变slot</button>
    </li>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
    slotName:'dddddd',
    data: ['zhangsan','lisi','wanwu','zhaoliu','tianqi','xiaoba']
  },
  methods: {
    changeSlot() {console.log('123');}

  }
}
</script>

<style scoped>

</style>
