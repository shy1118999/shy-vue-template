<!--
 * @Author: shaohang-shy
 * @Date: 2022-08-10 19:13:08
 * @LastEditors: shaohang-shy
 * @LastEditTime: 2022-08-31 18:44:41
 * @Description: Footer
-->
<script lang="ts" setup></script>

<template>
  <nav mt-6 inline-flex gap-2 text-xl>
    <button icon-btn @click="toggleDark()">
      <div i-carbon-sun dark:i-carbon-moon />
    </button>

    <a
      i-carbon-logo-github icon-btn
      rel="noreferrer"
      href="https://github.com/shy1118999/shy-vue-template"
      target="_blank"
      title="GitHub"
    />
  </nav>
</template>
