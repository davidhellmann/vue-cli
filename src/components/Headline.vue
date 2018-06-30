<script>
export default {
  name: 'Headline',
  render(h) {
    return h(this.size, this.text);
  },
  props: {
    size: String,
    text: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.headline {
  color: red;
}
</style>
