<template>
  <div class="home">
    <HelloWorld :color="dataColor">
      <div slot="app" slot-scope="user">slot--{{user.data}}</div>
    </HelloWorld>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  },
  data(){
    return {
      dataColor:'red',
      p:'123',
    slotName:'dddddd'

    }
  },
  mounted () {
    // console.log(p);
  }
}
</script>
