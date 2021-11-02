<template>
<div class="h-96">
    <page1-vue></page1-vue>
    <page2-vue></page2-vue>
    <page3-vue></page3-vue>
  </div>
</template>

<script>
import Page1Vue from "./page1.vue";
import Page2Vue from "./page2.vue";
import Page3Vue from "./page3.vue";
export default {
    components: {
        Page1Vue,
        Page2Vue,
        Page3Vue
    },
}
</script>
