<template>
  <div>
    <p>grand-child: <pre>{{ $attrs }}</pre>{{ $listeners }}</p>

    <button @click="$emit('myevent')">test $listeners</button>
  </div>
</template>



