<template>
  <div class="home">
    <button @click="onClick">AAAAAAAA</button>
    <img alt="Vue logo" src="../assets/logo.png">
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import Popup from '@/components/popup/Popup.vue'
import Vue from 'vue'
var ComponentClass = Vue.extend(Popup)

export default {
  name: 'home',
  components: {
    HelloWorld,
    Popup
  },
  methods: {
    onClick() {
        var instance = new ComponentClass({
            propsData: { type: 'primary' }
        })
        window.aaaa = instance;
        //instance.$slots.default = ['Click me!']
        instance.$mount() // pass nothing
//         console.log(this.$refs)
        document.body.appendChild(instance.$el)
      }
  }
}


</script>
