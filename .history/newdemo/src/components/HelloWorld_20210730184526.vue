<template>
  <div class="hello">
    <li>
        --{{$attrs.color}}
        <slot name="app" :data="data1"></slot>
        <button @click="changeSlot">改变slot</button>
        <!-- // 作用域插槽 -->
        <!-- <slot :data="data"></slot> -->
    </li>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
    slotName:'dddddd',

  },
  methods: {
    changeSlot() {console.log('123');}

  },
  data() {
    return {
      data1: ['zhangsan','lisi','wanwu','zhaoliu','tianqi','xiaoba']
    }
  }
}
</script>

<style scoped>

</style>
