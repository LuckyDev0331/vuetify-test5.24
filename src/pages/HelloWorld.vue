<template>
  <v-layout class="rounded rounded-md">
    <v-navigation-drawer class="px-3 py-4">
      <v-list-item class="list-card-group">
        <v-label style="color: #6F4E4E;">
          <svg
            width="39"
            height="39"
            viewBox="0 0 39 39"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M14.3 18.1996C12.576 18.1996 10.9227 17.5148 9.70376 16.2958C8.48477 15.0768 7.79995 13.4235 7.79995 11.6996V6.49961C7.79995 6.15483 7.93692 5.82417 8.18071 5.58037C8.42451 5.33657 8.75517 5.19961 9.09995 5.19961H10.4C10.7447 5.19961 11.0754 5.06265 11.3192 4.81885C11.563 4.57505 11.7 4.24439 11.7 3.89961C11.7 3.55483 11.563 3.22417 11.3192 2.98037C11.0754 2.73657 10.7447 2.59961 10.4 2.59961H9.09995C8.06561 2.59961 7.07363 3.0105 6.34223 3.74189C5.61084 4.47328 5.19995 5.46527 5.19995 6.49961V11.6996C5.20162 13.1683 5.55975 14.6146 6.24359 15.9143C6.92743 17.2141 7.91653 18.3284 9.12595 19.1616C10.2879 20.186 11.2303 21.4353 11.8961 22.834C12.5619 24.2327 12.9374 25.7518 13 27.2996C13 29.7131 13.9587 32.0277 15.6653 33.7343C17.3719 35.4409 19.6865 36.3996 22.1 36.3996C24.5134 36.3996 26.828 35.4409 28.5346 33.7343C30.2412 32.0277 31.2 29.7131 31.2 27.2996V25.8176C32.4254 25.5012 33.4934 24.7487 34.2037 23.7012C34.9141 22.6537 35.218 21.3831 35.0585 20.1275C34.899 18.872 34.2871 17.7177 33.3375 16.881C32.3878 16.0443 31.1656 15.5827 29.9 15.5827C28.6343 15.5827 27.4121 16.0443 26.4624 16.881C25.5128 17.7177 24.9009 18.872 24.7414 20.1275C24.5819 21.3831 24.8858 22.6537 25.5962 23.7012C26.3065 24.7487 27.3745 25.5012 28.6 25.8176V27.2996C28.6 29.0235 27.9151 30.6768 26.6961 31.8958C25.4772 33.1148 23.8239 33.7996 22.1 33.7996C20.376 33.7996 18.7227 33.1148 17.5038 31.8958C16.2848 30.6768 15.6 29.0235 15.6 27.2996C15.6658 25.7499 16.0453 24.2296 16.7157 22.8308C17.386 21.432 18.3332 20.1838 19.5 19.1616C20.7046 18.3255 21.6886 17.2099 22.3678 15.9103C23.047 14.6108 23.4012 13.166 23.4 11.6996V6.49961C23.4 5.46527 22.9891 4.47328 22.2577 3.74189C21.5263 3.0105 20.5343 2.59961 19.5 2.59961H18.2C17.8552 2.59961 17.5245 2.73657 17.2807 2.98037C17.0369 3.22417 16.9 3.55483 16.9 3.89961C16.9 4.24439 17.0369 4.57505 17.2807 4.81885C17.5245 5.06265 17.8552 5.19961 18.2 5.19961H19.5C19.8447 5.19961 20.1754 5.33657 20.4192 5.58037C20.663 5.82417 20.8 6.15483 20.8 6.49961V11.6996C20.8 12.5532 20.6318 13.3984 20.3052 14.1871C19.9785 14.9757 19.4997 15.6922 18.8961 16.2958C18.2926 16.8994 17.576 17.3782 16.7874 17.7048C15.9988 18.0315 15.1535 18.1996 14.3 18.1996ZM29.9 23.3996C29.2104 23.3996 28.5491 23.1257 28.0615 22.6381C27.5739 22.1505 27.2999 21.4892 27.2999 20.7996C27.2999 20.11 27.5739 19.4487 28.0615 18.9611C28.5491 18.4735 29.2104 18.1996 29.9 18.1996C30.5895 18.1996 31.2508 18.4735 31.7384 18.9611C32.226 19.4487 32.5 20.11 32.5 20.7996C32.5 21.4892 32.226 22.1505 31.7384 22.6381C31.2508 23.1257 30.5895 23.3996 29.9 23.3996Z"
              fill="#6F4E4E"
            />
          </svg>
          <b> ODP </b>
        </v-label>
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
    <v-app-bar class="pa-5">
      <div class="application-bar-content">
        <div class="search-input">
          <input
            type="search"
            style="background-color: #eff3f4; padding: 1%; border-radius: 20px"
            placeholder="Search"
          />
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
        <div style="padding-right: 20px">
          <v-avatar>
            <v-img
              alt="John"
              src="https://cdn.vuetifyjs.com/images/john.jpg"
            ></v-img>
          </v-avatar>
        </div>
      </div>
    </v-app-bar>
    <v-main
      class="d-flex align-center justify-center mt-6"
      style="min-height: 300px"
    >
      <v-container>
        <p style="font-size: 32px; color: #4d4d4d">
          Good Morning, Please check the orders
        </p>
        <v-tabs v-model="tab">
          <v-tab value="one">Orders</v-tab>
          <v-tab value="two">Reports</v-tab>
        </v-tabs>
        <v-row style="padding-top: 24px">
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
.application-bar-content {
  display: flex;
  gap: 20px;
  flex-direction: row;
  /* justify-content: space-around; */

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
