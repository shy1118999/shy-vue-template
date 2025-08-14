<!--
 * @Author: shaohang-shy
 * @Date: 2022-08-10 18:57:59
 * @LastEditors: shaohang-shy
 * @LastEditTime: 2023-04-06 08:58:46
 * @Description: index page
-->
<script setup lang="ts">
const name = ref('')

const router = useRouter()
function toSayHello() {
  if (name.value)
    router.push(`/hello/${encodeURIComponent(name.value)}`)
}
</script>

<template>
  <div>
    <p>Hello World!</p>
    <Counter :initial="0" />
    <div>
      <input v-model="name" placeholder="What's your name?" class="w-100 border border-gray-200 border-rounded bg-transparent px-4 py-2 text-center outline-none dark:border-gray-700 active:outline-none" @keydown.enter="toSayHello">
      <button class="mx-2 btn px-4 py-2" :disabled="!name" @click="toSayHello">
        Go
      </button>
    </div>
  </div>
</template>
