<script>
export default {
  props: {
    image: String,
    title: String,
    type: String,
  },
};
</script>

<template>
  <div class="col-comic">
    <div>
      <img :src="image" class="comic-cover" :alt="type">
    </div>
    <div>
      <span>{{ title }}</span>
    </div>
  </div>
</template>

<style scoped>
  span {
    color: white;
    text-transform: uppercase;
    margin-top: 10px;
    font-weight: 200;
    font-size: 0.7rem;
  }

  .col-comic{
    width: calc(100% / 6);
    padding: 0 10px;
  }

  .comic-cover{
    width: 100%;
    height: 180px;
  }
</style>