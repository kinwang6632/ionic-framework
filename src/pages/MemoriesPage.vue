<template>
  <base-layout page-title="All Memories" pageDefaultBackLink="/memories">
    <ion-list>
      <ion-item
        v-for="item in data"
        :key="item.id"
        router-link="/memories/{{item.id}}"
        >{{ item.title }}</ion-item
      >
    </ion-list>
  </base-layout>
</template>

<script setup lang="ts">
import { IonList, IonItem } from "@ionic/vue";
import { ref } from "vue";
const data = ref([
  { id: 1, title: "Max" },
  { id: 2, title: "Manuel" },
  { id: 3, title: "Julie" },
  { id: 4, title: "George" },
]); 
</script>

<style scoped>
ion-toolbar {
  --background: red;
}
</style>
