<template>
  <div class="hello">
    <li>
        --{{$attrs.color}}
        <slot name="app" :data="data1"></slot>
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
    changeSlot() {
      console.log('123');}
  },
  data() {
    return {
      data1: 'mjh'
    }
  },
  mounted () {
    console.log(this.$attrs);
  }
}
</script>

<style scoped>

</style>
