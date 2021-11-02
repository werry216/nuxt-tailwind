<template>
  <div class="grid grid-cols-3 gap-2  0 m-10">
    <index1-vue></index1-vue>
    <index2-vue></index2-vue>
    <index3-vue></index3-vue>
  </div>
</template>

<script>
import Index1Vue from "~/components/index1";
import Index2Vue from "~/components/index2";
import Index3Vue from "~/components/index3";
export default {
  components: {
    Index1Vue,
    Index2Vue,
    Index3Vue
  }
}
</script>
