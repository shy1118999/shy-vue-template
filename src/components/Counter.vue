<!--
 * @Author: shaohang-shy
 * @Date: 2022-08-11 09:14:44
 * @LastEditors: shaohang-shy
 * @LastEditTime: 2022-08-11 09:17:32
 * @Description: Counter
-->
<script setup lang="ts">
const props = defineProps<{
  initial: number
}>()
const { count, inc, dec } = useCounter(props.initial)
</script>

<template>
  <div class="m-5">
    <div>
      {{ count }}
    </div>
    <div>
      <button class="btn m-2" @click="inc()">
        +
      </button>
      <button class="btn m-2" @click="dec()">
        -
      </button>
    </div>
  </div>
</template>
