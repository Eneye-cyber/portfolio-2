<script setup lang="ts">
import { computed } from 'vue';


const props = defineProps<{ secondary?: Boolean }>()

const classGroup = computed(() => {
  return props.secondary ? 'btn btn_secondary' : 'btn btn_primary'
})
</script>

<template>
  <a href="#" :class="classGroup">
    <slot>Submit</slot>
  </a>
</template>

<style scoped>
.btn{
  display: inline-flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  padding: 16px 10px;
  gap: 10px;
  position: relative;
  width: 200px;
  height: 53px;

  border-radius: 8px;
  box-sizing: border-box;
  font-weight: 400;
  font-size: 18px;
  line-height: 21px;
  text-transform: capitalize;
  text-decoration: none;
  margin: 0 10px;
}
.btn_primary{
  background: #2BA6C1;
  border: 1px solid #2BA6C1;
  color: #FFFFFF;
}
.btn_secondary{
  background: transparent;
  border: 1.7px solid #2BA6C1;
  color: #2BA6C1;
}
</style>
