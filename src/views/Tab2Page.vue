<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Spielinformation:</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Tab 2</ion-title>
        </ion-toolbar>
      </ion-header>
      <ion-input type="number" >Spieleranzahl</ion-input>
      <p>Bahnen</p>
      <ion-list>
    <ion-radio-group value="biff">
      <ion-item>
        <ion-label>Hauptbahn</ion-label>
        <ion-radio slot="start" value="biff"></ion-radio>
      </ion-item>

      <ion-item>
        <ion-label>Nebenbahn</ion-label>
        <ion-radio slot="start" value="griff"></ion-radio>
      </ion-item>

    </ion-radio-group>
  </ion-list>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent } from '@ionic/vue';

export default defineComponent({
  name: 'Tab2Page',
  components: {IonHeader, IonToolbar, IonTitle, IonContent, IonPage }
});
</script>

<style>

</style>
