<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-buttons slot="start">
          <ion-menu-button color="primary"></ion-menu-button>
        </ion-buttons>
        <ion-title>Tab 1</ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Tab 1</ion-title>
        </ion-toolbar>
      </ion-header>

      <ion-list>
        <ion-item v-for="i in 30" :key="i">
          <ion-title>{{ i }}</ion-title>
          <ion-text>Number</ion-text>
        </ion-item>
      </ion-list>
    </ion-content>
  </ion-page>
</template>

<script>
import {
  IonPage,
  IonHeader,
  IonToolbar,
  IonTitle,
  IonContent,
  IonList,
  IonItem,
  IonText,
  IonButtons,
  IonMenuButton,
} from "@ionic/vue";

export default {
  name: "Tab1",
  components: { 
    IonHeader, 
    IonToolbar, 
    IonTitle, 
    IonContent, 
    IonPage,
    IonList,
    IonItem,
    IonText,
    IonButtons,
    IonMenuButton,
  },
};
</script>