<template>
  <li class="flex flex-col items-center cursor-pointer w-20 sm:w-20 hover:text-white group">
    <Icon class="h-8 mb-1 group-hover:animate-bounce" />
    <a href="#" class="uppercase">{{ name }}</a>
  </li>
</template>

<script setup lang="ts">
import type { FunctionalComponent, HTMLAttributes, VNodeProps } from 'vue'
const props = defineProps<{
  name: String
  Icon: FunctionalComponent<HTMLAttributes & VNodeProps, {}, any>
}>()
</script>
