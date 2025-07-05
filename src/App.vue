<template>
  <v-app>
    <v-app-bar app color="white" light>
      <v-toolbar-title class="ml-4">
        <v-img src="/Genshin_Impact_Logo.png" max-height="30" contain></v-img>
      </v-toolbar-title>

      <v-spacer></v-spacer>

      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn text to="/">Home</v-btn>
        <v-btn text to="/search">Search</v-btn>
        <v-btn text to="/message">Message</v-btn>
        <v-divider vertical class="mx-2"></v-divider>
        <v-btn text>Log In</v-btn>
        <v-btn color="primary">Sign Up</v-btn>
      </v-toolbar-items>

      <v-app-bar-nav-icon class="hidden-md-and-up"></v-app-bar-nav-icon>

      <v-btn icon class="ml-2">
        <v-icon>mdi-account-outline</v-icon>
      </v-btn>
      <v-btn icon>
        <v-icon>mdi-plus</v-icon>
      </v-btn>

    </v-app-bar>

    <v-main>
      <router-view /> </v-main>

    <v-footer app>
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: 'App',
};
</script>

<style>
/* คุณสามารถเพิ่ม Global Styles ที่นี่ */
/* กำหนดสีพื้นหลังหลักของ v-app ให้เป็นสีอ่อนๆ */
.v-application {
  background-color: #F8F9FA !important; /* สีเทาอ่อน */
}

/* เพิ่ม styles สำหรับ v-app-bar-nav-icon ถ้าคุณใช้มัน */
.v-app-bar-nav-icon {
  margin-right: 0px !important; /* ลบระยะห่างด้านขวาถ้าต้องการให้โลโก้ชิดซ้ายสุด */
}
</style>