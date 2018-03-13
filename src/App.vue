<template>
  <div id="app">
    <child :myprop="myprop" @myevent="myevent"></child>
  </div>
</template>

<script>
export default {
  components: { child: () => import('./components/Child') },

  data () {
    return {
      myprop: {
        a: 'a',
        b: 'b'
      }
    }
  },

  methods: {
    myevent () {
      console.log('event received')
    }
  }
}
</script>

