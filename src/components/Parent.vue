<template>
  <div>
    <p>parent: <pre>{{ $attrs }}</pre></p>

    <grand-child v-bind="$attrs" v-on="$listeners"></grand-child>
  </div>
</template>

<script>
export default {
  components: { grandChild: () => import('./GrandChild') }
}
</script>
