<template>
<ion-page>
  <ion-header>
    <IonToolbar>
      <ion-buttons slot="start">
        <ion-menu-button color="primary"/>
      </ion-buttons>
      <ion-title>Cards</ion-title>
    </IonToolbar>
  </ion-header>
  <ion-content :fullscreen="true">
    <ion-header collapse="condense">
      <ion-toolbar>
        <ion-title size="large">Cards</ion-title>
      </ion-toolbar>
    </ion-header>

    <div id="container">
      <ion-card>
        <img alt="Silhouette of mountains" src="https://ionicframework.com/docs/img/demos/card-media.png" />
        <ion-card-header>
          <ion-card-title>Card Title</ion-card-title>
          <ion-card-subtitle>Card-subtitle</ion-card-subtitle>
        </ion-card-header>
        <ion-card-content>
          This is the card content
        </ion-card-content>
      </ion-card>
    </div>
  </ion-content>
</ion-page>
</template>

<script lang="ts" setup>
import {IonPage, IonHeader, IonToolbar, IonCard} from "@ionic/vue"
</script>

<style scoped>
#container {
  text-align: center;
  position: absolute;
  left: 0;
  right: 0;
  top: 50%;
  transform: translateY(-50%);
}

#container strong {
  font-size: 20px;
  line-height: 26px;
}

#container p {
  font-size: 16px;
  line-height: 22px;
  color: #8c8c8c;
  margin: 0;
}

#container a {
  text-decoration: none;
}
</style>