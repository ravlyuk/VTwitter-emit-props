<template>
  <ul class="tweets__wrapper">
    <Item
        v-for="item in items"
        :key="item.id"
        :item="item"
    />
  </ul>
</template>

<script>

import Item from "@/components/Item.vue"


export default {
  components: {Item},
  name: "List",
  props: {
    items: {
      type: Array,
      required: true,
    }
  }

}
</script>

<style scoped>

</style>