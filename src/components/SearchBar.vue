<template>
  <div>
    <input @termChange="onInput" />
  </div>
</template>

<script>
export default {
  name: 'SearchBar',
  methods: {
    onInput: function(event) {
      this.$emit('termChange', event.target.value);
    },
  },
};
</script>

<style>

</style>
