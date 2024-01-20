<template>
  <div class="screen">
    <h1>Poke Memories</h1>
    <h3>Select mode to start game</h3>
    <div class="action">
      <button @click="onStart(16)">
        <span>4*4</span>
        <span>Easy</span>
      </button>
      <button @click="onStart(36)">
        <span>6*6</span>
        <span>Medium</span>
      </button>
      <button @click="onStart(64)">
        <span>8*8</span>
        <span>Hard</span>
      </button>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    onStart(totalOfBlocks) {
      this.$emit("onStart", { totalOfBlocks });
    }
  }
}
</script>
