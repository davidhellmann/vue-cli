<template>
  <div class="cards">
    <h2>This is an Cards Component</h2>
    <div class="cards__list">
      <div class="cards__item" v-for="index in 10" :key="index">
        <card :counter="index">
          Loop-{{ index }}
        </card>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Card from '@/components/molecules/Card.vue';

export default {
  name: 'Cards',
  components: {
    Card,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.cards {
  width: 100%;

  &__list {
    display: flex;
    flex-flow: row wrap;
    justify-content: flex-start;
    align-items: flex-start;
  }

  &__item {
    width: 33%;
    flex: 1 1 33%;
    padding: 16px;
    box-sizing: border-box;
  }
}
</style>
