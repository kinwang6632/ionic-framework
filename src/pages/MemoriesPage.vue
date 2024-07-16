<template>
  <h2>Memories Page</h2>
  <ion-page>
    <ion-header>
      <ion-toolbar color="primary">
        <ion-title>All Memories</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content>
      <ion-list>
        <ion-item>Max</ion-item>
        <ion-item>Manuel</ion-item>
        <ion-item>Julie</ion-item>
        <ion-item>George</ion-item>
      </ion-list>
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import {
  IonContent,
  IonHeader,
  IonToolbar,
  IonPage,
  IonTitle,
  IonList,
  IonItem,
  
} from "@ionic/vue";
</script>

<style scoped>
    ion-toolbar {
        --background:red;
    }
</style>
