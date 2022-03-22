<template>
  <AccordionItem v-if="attribute" :heading="attribute.name">
    <!-- eslint-disable vue/no-v-html -->
    <div class="pb-3" v-html="attribute.value" />
    <!--eslint-enable-->
  </AccordionItem>
</template>

<script>
export default {
  props: {
    attribute: {
      type: Object,
      default: () => {},
    },
  },
}
</script>
