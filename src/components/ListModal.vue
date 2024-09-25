<script setup>
//default is optional and can receive any type
//const props = defineProps(['items', 'format'])
// const props = defineProps({
//     items: {
//         type: Array,
//         Required: true
//     },
//     format: {
//         type: String,
//         Validator(value) {
//             // The value must match one of these strings
//             return ['card', 'list', 'box'].includes(value)
//         }
//     } //Array, Obj, Boolean
// })

const props = defineProps({
    list: {
        type: Array,
        required: true
    }
})

</script>

<template>
  <div>
    <slot v-for="(group, index) in list", :key="index" :listGroup="group"></slot>
  </div>
</template>

<style scoped></style>