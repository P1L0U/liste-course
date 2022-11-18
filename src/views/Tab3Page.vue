<!--<template>
  <ion-page>
    <ion-header>
    <ion-title>Ma liste de course</ion-title>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense"></ion-header>
      <ion-item>
        <ion-label position="floating">Entrer un produit</ion-label>
        <ion-input type="email" v-model="produit" required></ion-input>
      </ion-item>
      <ion-button color="primary" @click="Listeajout()">Ajouter à la liste</ion-button>
    </ion-content>
  </ion-page>
</template>

<script>
import {defineComponent} from 'vue';
import { IonPage, IonHeader, IonInput, IonButton, IonItem, IonLabel, IonTitle } from '@ionic/vue';
import Todolist from '.components/Todolist'

export default defineComponent({
  name: 'Tab3Page',
  components: { IonHeader, IonPage, IonInput, IonButton, IonItem, IonLabel, IonTitle },
});
</script>!-->
<template>
  <div id="app" class="container">
    <todo-list></todo-list>
  </div>
</template>

<script>
import TodoList from './components/TodoList'
export default {
  name: 'Tab3Page',
  components: {
    TodoList,
  }
}
</script>

<style>
* {
  box-sizing: border-box;
}
.container {
  max-width: 600px;
  margin: 0 auto;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  margin-top: 60px;
  font-size: 24px;
}
.logo {
  display: block;
  margin: 20px auto;
  height: 75px;
}
</style>