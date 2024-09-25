<script setup></script>

<template>
  <div
    class="flex flex-col items-center justify-center text-black h-20"
  >
    <!-- slot outlet -->
    <!-- Default fallback content -->
    <div class="text-4xl font-semibold">
      <slot name="firstLineHeader"></slot>
    </div>
    <div class="text-2xl">
      <slot name="secondLineHeader"></slot>
    </div>
  </div>
</template>

<style scoped></style>