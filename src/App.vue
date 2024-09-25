<script setup>
import Header from './components/Header.vue'
import GroupList from './components/GroupList.vue'
</script>

<template>
  <div>
    <!-- slot content -->
    <Header>
      <template v-slot:firstLineHeader>
        <h1>School of Information Technology</h1>
      </template>
      <template #secondLineHeader>
        <!-- v-slot: has same meaning #  -->
        <h2>King's Mongut University of Technology Thonburi</h2>
      </template>
    </Header>
    <GroupList></GroupList>
  </div>
</template>

<style scoped></style>