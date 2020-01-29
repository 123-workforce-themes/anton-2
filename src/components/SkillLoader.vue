<template>
  <main id="skills">
    <slot></slot>
    <div class="skill-level" :style="`background: ${background}; width: ${width}%`">
      <div class="bar"></div>
    </div>
  </main>
</template>

<script>
export default {
  props: {
   background: String,
   width: Number
  }
}
</script>

<style scoped>

#skills {
  display: grid;
  grid-template-columns: auto 1fr;
  width: 40%;
  margin: auto;
  grid-gap: 1rem;
  padding: 25px 0px;
}

#skills .skill-img {
  padding-right: 42px;
}

#skills .skill-level {
  position: relative;
  border-radius: 9px;
  height: 5px;
  margin-top: 20px;
  margin-left: 48px;
}

#skills .skill-level .bar {
  position: absolute;
  background: blue;
  left: 0;
}
</style>