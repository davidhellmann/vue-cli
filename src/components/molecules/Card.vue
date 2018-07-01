<template>
  <div class="card">
    <Headline :text="`Headline ${counter}`" size="h3"></Headline>
    <p>lorem ipsum dolor sit amet</p>
  </div>
</template>

<script>
// @ is an alias to /src
import Headline from '@/components/atoms/Headline.vue';

export default {
  name: 'Card',
  props: {
    counter: String,
    size: String,
  },
  components: {
    Headline,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.card {
  width: 100%;
  border: 1px solid #ddd;
  border-radius: 5px;
}
</style>
