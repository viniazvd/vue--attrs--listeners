<template>
  <div>
    <p>grand-child: <pre>{{ $attrs }}</pre></p>

    <button @click="$emit('myevent')">test $listeners</button>
  </div>
</template>



