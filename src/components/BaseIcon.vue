<template>
  <div class="icon-wrapper">
    <svg class="icon" width="width" height="height"></svg>
    <use v-bind="{ 'xlink:href': '/feather-sprite.svg#' + name }" />
  </div>
</template>

<script>
export default {
  props: {
    name: String,
    width: {
      type: [Number, String],
      default: 24
    },
    height: {
      type: [Number, String],
      default: 24
    }
  }
};
</script>

<style></style>
