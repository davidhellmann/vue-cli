<template>
  <div class="test">
    <h1>This is an test page</h1>
    <Test msg="paioshjd aish dpiah dpiah dipah dip" headline="Test" />
  <cards></cards>
  </div>
</template>

<script>
// @ is an alias to /src
import Test from '@/components/organisms/Test.vue';
import Cards from '@/components/organisms/Cards.vue';

export default {
  name: 'test',
  components: {
    Test,
    Cards,
  },
};
</script>
