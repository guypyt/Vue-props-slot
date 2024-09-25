<script setup>
import Header from './Header.vue';
import groups from '../../data/groups.json'
import ListModal from './ListModal.vue'
</script>

<template>
  <div>
    <!-- <ListModal :items="products" v-slot="slotProps">
        <div class="p-5 shadow-lg w-1/3">
            <p>{{ slotProps.lineItem.productName }}</p>
            <p>{{ slotProps.lineItem.price }}</p>
        </div>
    </ListModal> -->

    <Header>
        <template #secondLineHeader><< Group List >></template>
    </Header>

    <ListModal :list="groups" v-slot="slotProps">
    <div class="p-5 shadow-lg w-1/3">
        <p>{{ slotProps.listGroup.groupName }}</p>
        <p>{{ slotProps.listGroup.repo }}</p>
    </div>
</ListModal>

  </div>
</template>

<style scoped></style>