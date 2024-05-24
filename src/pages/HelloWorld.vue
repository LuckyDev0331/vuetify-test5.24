<template>
  <v-layout class="rounded rounded-md">
    <v-navigation-drawer>
      <v-list-item title="My Application" subtitle="Vuetify">
        <div> ddd </div>
        <div> ddd </div>

        <div> ddd </div>

      </v-list-item>
      <v-divider></v-divider>
      
      <v-list-item link title="Dashboard"></v-list-item>
      <v-list-item link title="Patient List"></v-list-item>
      <v-list-item link title="General File"></v-list-item>
    </v-navigation-drawer>

    <v-app-bar>
      <div>
        <input type="search" placeholder="Search" />
      </div>
    </v-app-bar>

    <v-main
      class="d-flex align-center justify-center"
      style="min-height: 300px"
    >
      <v-container>
        <v-label> Good Morning, Please check the orders </v-label>
        <v-tabs v-model="tab">
          <v-tab value="one">Orders</v-tab>
          <v-tab value="two">Reports</v-tab>
        </v-tabs>
        <v-row>
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
