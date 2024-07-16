<template>
  <ion-page>
    <ion-header>
      <ion-toolbar color="primary">
        <ion-buttons slot="start">
          <ion-back-button :default-href="props.pageDefaultBackLink"></ion-back-button>
        </ion-buttons>
        <ion-title>{{ props.pageTitle }} </ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content>
      <slot></slot>
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
  IonBackButton,
  IonButtons,
} from "@ionic/vue";

const props = defineProps({
  pageTitle: {
    type: String,
    default: "Base Layout",
  },
  pageDefaultBackLink: {
    type: String,
    default: "/",
  }
});
</script>

<style scoped></style>
