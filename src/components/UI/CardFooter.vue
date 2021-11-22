<template>
  <div class="card-stats">
    <div
      v-for="(stat, index) in data"
      :key="index"
      class="one-third"
    >
      <div class="stat-value">{{ stat[item_value] }}</div>
      <div class="stat">{{ stat[item_key] }}</div>
    </div>
  </div>
</template>
<script>
export default {
  props: {
    data: {
      type: Array,
      required: true
    },
    item_key: {
      type: String,
      required: true
    },
    item_value: {
      type: String,
      required:true
    }
  }
}
</script>
