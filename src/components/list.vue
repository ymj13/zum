<template>
  <div class="week-info-list">
    <div class="date">
      <span>월 5.16</span>
    </div>
    <ul class="accordion">
      <li>
        <div class="accorion-header">

        </div>
        <div class="accordion-content">

        </div>
      </li>
    </ul>
  </div>
</template>

<script>

export default {
  name: 'week-info-list',
  props: {
    data: {
      type: Array,
      default: null
    }
  }
}
</script>

<style>

</style>