<template>
  <div class="ni-field-group">
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: 'ni-field-group'
}
</script>

<style lang="stylus">
@import '../styles/variables.styl'

.ni-field-group
  display flex
  margin-bottom 0.5rem
  max-width 40rem

  .ni-field
    flex 1

  .ni-field-addon
    width 2rem

  .ni-field, .ni-btn-wrapper
    margin 0

  .ni-btn-wrapper
    max-width 15rem

  .ni-field + .ni-btn-wrapper
    margin-left 1rem

  .ni-btn-wrapper + .ni-field
    margin-left 1rem

  .ni-field-addon
    background c-app-bg
    border 1px solid #ccc
    display flex
    align-items center
    padding 0 0.5rem
    height 2rem

    color light

  .ni-field + .ni-field-addon
    border-left none

  .ni-field-addon + .ni-field
    border-left none

@media screen and (min-width: 768px)
  .ni-field-group
    margin-bottom 0.75rem
</style>
