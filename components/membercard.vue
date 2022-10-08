<template>
  <v-container grid-list-xs>
    <v-card>
      <v-img
        src="https://i.natgeofe.com/k/75ac774d-e6c7-44fa-b787-d0e20742f797/giant-panda-eating_3x2.jpg"
      ></v-img>
      <v-card-title class="d-flex justify-center" primary-title>
        Б.Зуунбилэг
      </v-card-title>
      <v-divider class="mx-4"></v-divider>
      <v-card-subtitle class="text-center"
        >Дэлгэрэнгүй
        <v-icon color="green "
          >mdi-card-account-details-outline</v-icon
        ></v-card-subtitle
      >
      <v-card-text>
        UI/UX figma дээр жоохоон л Веб - C, C++ - html, css, javascript - react
        - nodejs - express - mongo/mysql - typing - бие дааж сурах зөвлөгөө өгөх
        (source-ууд) - мотивацжуулах - англи хэл - чадвар дээрээ суурилан хичээл
        заах
      </v-card-text>
      <v-expansion-panels>
        <v-expansion-panel elevation="0">
          <v-expansion-panel-header class="green--text"
            ><div>
              Багийн гишүүд
              <v-icon color="green ">mdi-card-account-details-outline</v-icon>
            </div>
          </v-expansion-panel-header>
          <v-expansion-panel-content
            ><v-form>
              <v-text-field
                label="Таны нэр"
                single-line
                color="green"
              ></v-text-field>
              <v-text-field
                label="Таны утасны дугаар"
                single-line
                color="green"
              ></v-text-field>
            </v-form>
            <div v-if="!sanal" class="d-flex justify-center pa-10">
              <v-btn color="green" @click="(sanal = !sanal), (helo = !helo)"
                >Багт нэгдэх</v-btn
              >
            </div>
          </v-expansion-panel-content>

          <v-snackbar v-model="helo">
            {{ text }} <v-icon color="green">mdi-account-check</v-icon>

            <template v-slot:action="{ attrs }">
              <v-btn color="pink" text v-bind="attrs" @click="helo = !helo">
                Cool
              </v-btn>
            </template>
          </v-snackbar>
          <div v-if="sanal" class="d-flex justify-center">
            <v-card-title primary-title color="green">
              Та санал өгсөн байна <v-icon>mdi-check-decagram</v-icon>
            </v-card-title>
          </div>
        </v-expansion-panel>
      </v-expansion-panels>
    </v-card>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      sanal: false,
      helo: false,
      text: `Таны саналыг хүлээн авлаа`,
    };
  },
};
</script>

<style></style>
