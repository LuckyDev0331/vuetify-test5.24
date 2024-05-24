<template>
  <v-layout class="rounded rounded-md">
    <v-navigation-drawer>
      <v-list-item class="list-card-group" title="ODP">
        <v-sheet class="d-flex flex-wrap">
          <v-sheet class="flex-1-0-100 ma-2 pa-2">
            Remainder for doctor
          </v-sheet>
          <v-sheet class="flex-1-1 ma-2 pa-2"> History </v-sheet>
          <v-sheet class="ma-2 pa-2"> pending </v-sheet>
          <v-sheet class="flex-1-2 ma-2 pa-2"> medication </v-sheet>
          <v-sheet class="ma-2 pa-2"> pending </v-sheet>
        </v-sheet>
      </v-list-item>
      <v-divider></v-divider>

      <v-list-item link title="Dashboard"></v-list-item>
      <v-list-item link title="Patient List"></v-list-item>
      <v-list-item link title="General File"></v-list-item>
    </v-navigation-drawer>
    <v-app-bar class="application-bar">
      <div class="application-bar-content">
        <div class="search-input">
          <input type="search" style="background-color: #EFF3F4; padding: 2%; border-radius: 20px" placeholder="Search" />
        
        </div>
        <div class="appointments"><p>Appointments</p></div>
        <div>
          <svg
            width="20"
            height="25"
            viewBox="0 0 20 25"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M10 24.5C11.375 24.5 12.5 23.375 12.5 22H7.5C7.5 23.375 8.625 24.5 10 24.5ZM17.5 17V10.75C17.5 6.9125 15.4625 3.7 11.875 2.85V2C11.875 0.9625 11.0375 0.125 10 0.125C8.9625 0.125 8.125 0.9625 8.125 2V2.85C4.55 3.7 2.5 6.9 2.5 10.75V17L0 19.5V20.75H20V19.5L17.5 17ZM15 18.25H5V10.75C5 7.65 6.8875 5.125 10 5.125C13.1125 5.125 15 7.65 15 10.75V18.25Z"
              fill="#6B6B6B"
            />
          </svg>
        </div>
        <v-avatar>
          <v-img
            alt="John"
            src="https://cdn.vuetifyjs.com/images/john.jpg"
          ></v-img>
        </v-avatar>
      </div>
    </v-app-bar>
    <v-main
      class="d-flex align-center justify-center"
      style="min-height: 300px"
    >
      <v-container>
        <p style="font-size: 32px; color: #4D4D4D"> Good Morning, Please check the orders </p>
        <v-tabs v-model="tab">
          <v-tab value="one">Orders</v-tab>
          <v-tab value="two">Reports</v-tab>
        </v-tabs>
        <v-row style="padding-top: 24px;">
          <v-col cols="12" md="3" v-for="index in 16" :key="`block-${index}`">
            <BlockCmp :labelText="labelText[index]" />
          </v-col>
        </v-row>
      </v-container>
    </v-main>
  </v-layout>
</template>

<script>
import logo from "../assets/logo.svg";
import BlockCmp from "../components/BlockComponent.vue";

export default {
  name: "HelloWorld",

  components: {
    BlockCmp,
  },
  data() {
    return {
      labelText: [
        "Labs",
        "Biopsy FNA",
        "day procedure",
        "Office procedure",
        "imaging",
        "fuctional tests",
        "Medications",
        "Office procedure",
        "Labs",
        "Biopsy FNA",
        "day procedure",
        "Office procedure",
        "Labs",
        "Biopsy FNA",
        "day procedure",
        "Office procedure",
        "Labs",
      ],
    };
  },
};
</script>
<style scoped lang="css">
.list-card-group {
  display: flex;
  flex-direction: row;
}

.list-card {
  background-color: #f6f1f1;
  margin: 5px;
}
.application-bar {
  padding-left: 2%;
  padding-right: 2%;
}
.application-bar-content {
  display: flex;
  flex-direction: row;
  justify-content: space-around;

  width: 100%;
}
.search-input {
  flex-grow: 1;
}
.appointments {
  display: flex;
  text-align: center;
  justify-content: center;
  align-items: center;
  margin-left: 20%;

  background-color: #a18080;
  width: 170px;
  height: 62px;
  color: white;
}
</style>
