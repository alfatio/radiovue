<template>
  <div>
  <input type="radio" :name=name>
  <slot></slot>
  </div>
</template>

<script>
export default {
  props: ['name']
}
</script>

<style>

</style>