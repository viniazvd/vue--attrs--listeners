<template>
  <div>
    <p>child: <pre>{{ $attrs }}</pre></p>

    <parent v-bind="$attrs" v-on="$listeners"></parent>
  </div>
</template>

<script>
export default {
  components: { parent: () => import('./Parent') }
}
</script>
