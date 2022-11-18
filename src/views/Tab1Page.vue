<template>
  <ion-page>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense"></ion-header>
      <ion-item>
        <ion-label position="floating">Nom</ion-label>
        <ion-input type="text" v-model="nom" required></ion-input>
      </ion-item>
      <ion-item>
        <ion-label position="floating">Prénom</ion-label>
        <ion-input type="text" v-model="prenom" required></ion-input>
      </ion-item>
      <ion-item>
        <ion-label position="floating">Email</ion-label>
        <ion-input type="email" v-model="email" required></ion-input>
      </ion-item>
      <ion-item>
        <ion-label position="floating">Mot de passe</ion-label>
        <ion-input type="password" v-model="password" required></ion-input>
      </ion-item>
      <ion-button color="primary" @click="Inscription()">Inscription</ion-button>

      <ion-button color="primary" @click="Connexion()">Connexion</ion-button>
    </ion-content>
  </ion-page>
</template>

<script>
import { defineComponent} from 'vue';
import { IonPage, IonHeader, IonContent, IonInput, IonItem, IonLabel, IonButton } from '@ionic/vue';

export default defineComponent({
  name: 'Tab1Page',
  components: {IonHeader, IonContent, IonPage, IonInput, IonItem, IonLabel, IonButton },
});
</script>
