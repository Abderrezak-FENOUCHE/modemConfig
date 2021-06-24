<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Home</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-grid>
        <ion-row>
          <ion-col class="ion-text-center" size="4">
            <ion-icon :icon="wifi" />
          </ion-col>
          <ion-col class="ion-text-center" size="4">
            <ion-row>
              <ion-col size="12">
                Etat wifi
              </ion-col>
              <ion-col size="12">
                0.0.0.0
              </ion-col>
              <ion-col size="12">
                192.168.5.3
              </ion-col>
            </ion-row>
          </ion-col>
          <ion-col class="ion-text-center" size="4">
             {{battery}} %
          </ion-col>
        </ion-row>
        <ion-row>
          <ion-col class="ion-text-center" size="4">
            <ion-icon name="add-circle-outline"></ion-icon>
            Mhz
          </ion-col>
          <ion-col class="ion-text-center" size="4">
                <ion-icon :icon="wifi" />
          </ion-col>
          <ion-col class="ion-text-center" size="4">
            mbps
          </ion-col>
        </ion-row>
        <ion-row>
          <ion-col class="ion-text-center" size="4">
            <ion-icon name="add-circle-outline"></ion-icon>
            <ion-icon name="md-add"></ion-icon>
            Paramètre wifi
          </ion-col>
          <ion-col class="ion-text-center" size="4">
                Les Mot de passe
          </ion-col>
          <ion-col class="ion-text-center" size="4">
            Scanner Wifi
          </ion-col>
        </ion-row>
        <ion-row>
          <ion-col class="ion-text-center" size="6">
            <ion-icon name="add-circle-outline"></ion-icon>
            Aidez-moi
          </ion-col>
          <ion-col class="ion-text-center" size="6">
            Ping
          </ion-col>
        </ion-row>
        
      </ion-grid>
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
  IonIcon,
  IonCol,
  IonGrid,
  IonRow,
} from "@ionic/vue";
import { wifi } from "ionicons/icons";
export default {
  name: "Tab1",
  components: {
    IonHeader,
    IonToolbar,
    IonTitle,
    IonContent,
    IonPage,
    IonIcon,
    IonCol,
    IonGrid,
    IonRow,
  },
 data: () => ({
    battery : 50
  }),

  setup() {
    return {
      wifi
    };
  },
};
</script>