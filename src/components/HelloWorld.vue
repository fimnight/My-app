<template>
  <v-container fluid class="pa-6">
    <v-card class="hero-card pa-0 rounded-xl elevation-0 mb-8" color="#E6F0FF">
      <v-row no-gutters align="center">
        <v-col cols="12" md="7" class="pa-6">
          <v-img src="/genshin-logo-mini.png" max-height="25" contain position="left" class="mb-4"></v-img>
          <div class="text-h4 font-weight-bold mb-2">Layla</div>
          <p class="text-subtitle-1 grey--text text--darken-2 mb-4">
            She is a student in the Rtawahist Darshan,<br>
            specializing in Theoretical Astrology.
          </p>
          <v-btn color="#99CCFF" dark large rounded>Read More</v-btn>
        </v-col>
        <v-col cols="12" md="5" class="d-flex align-end justify-end">
          <v-img src="/layla-hero.png" contain max-height="300" class="hero-image"></v-img>
        </v-col>
      </v-row>
    </v-card>

    <v-row>
      <v-col cols="12" md="7">
        <div class="d-flex justify-space-between align-center mb-4">
          <div class="text-h6 font-weight-bold">Artwork</div>
          <v-btn text small color="primary">
            View More
            <v-icon right>mdi-chevron-right</v-icon>
          </v-btn>
        </div>
        <v-row>
          <v-col cols="6" sm="4" md="4" lg="3">
            <v-card class="artwork-card rounded-lg elevation-0">
              <v-img src="/artwork1.jpg" aspect-ratio="1" class="rounded-lg"></v-img>
              <div class="text-caption grey--text text--darken-1 text-center py-2">by @sukacchi</div>
            </v-card>
          </v-col>
          <v-col cols="6" sm="4" md="4" lg="3">
            <v-card class="artwork-card rounded-lg elevation-0">
              <v-img src="/artwork2.jpg" aspect-ratio="1" class="rounded-lg"></v-img>
              <div class="text-caption grey--text text--darken-1 text-center py-2">by @RenChain</div>
            </v-card>
          </v-col>
          </v-row>
      </v-col>

      <v-col cols="12" md="5">
        <div class="text-h6 font-weight-bold mb-4">Recent Search</div>
        <v-card class="recent-search-card pa-4 rounded-xl elevation-0 mb-6">
          <v-chip-group column>
            <v-chip class="custom-chip" close>
              <v-icon left>mdi-magnify</v-icon> Layla ascension material
            </v-chip>
            <v-chip class="custom-chip" close>
              <v-icon left>mdi-magnify</v-icon> Layla build
            </v-chip>
            <v-chip class="custom-chip" close>
              <v-icon left>mdi-magnify</v-icon> kalpalata lotus locations
            </v-chip>
            <v-chip class="custom-chip" close>
              <v-icon left>mdi-magnify</v-icon> Layla cosplay
            </v-chip>
            <v-chip class="custom-chip" close>
              <v-icon left>mdi-magnify</v-icon> Layla Wallpaper
            </v-chip>
          </v-chip-group>
        </v-card>

        <v-row>
          <v-col cols="12" sm="6">
            <v-card class="info-card pa-4 rounded-xl elevation-0 text-center">
              <v-avatar size="64" class="mb-2">
                <v-img src="/cryo-icon.png"></v-img>
              </v-avatar>
              <div class="text-h6 font-weight-bold">Cryo character</div>
              <div class="text-caption grey--text text--darken-1">The elemental skill for the character is ...</div>
            </v-card>
          </v-col>
          <v-col cols="12" sm="6">
            <v-card class="info-card pa-4 rounded-xl elevation-0 text-center">
              <v-avatar size="64" class="mb-2">
                <v-img src="/sumeru-icon.png"></v-img>
              </v-avatar>
              <div class="text-h6 font-weight-bold">Sumeru</div>
              <div class="text-caption grey--text text--darken-1">Sumeru is one of the seven regions of Teyvat. It is known for its vast ...</div>
            </v-card>
          </v-col>
          <v-col cols="12">
            <v-card class="info-card pa-4 rounded-xl elevation-0">
              <v-avatar size="64" class="mb-2 mr-4 float-left">
                <v-img src="/akademiya-icon.png"></v-img>
              </v-avatar>
              <div class="text-h6 font-weight-bold">Akademiya</div>
              <div class="text-caption grey--text text--darken-1">The Sumeru Akademiya is Sumeru's main governing body, as well as the ...</div>
            </v-card>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'HomeView',
}
</script>

<style scoped>
.hero-card {
  background: linear-gradient(to right, #E6F0FF, #CCEEFF); /* Adjust gradient colors */
  position: relative;
  overflow: hidden;
}

.hero-image {
  position: absolute;
  right: 0;
  bottom: 0;
  max-width: 100%; /* Ensure image fits within its container */
  height: auto;
}

.hero-card .v-btn {
  text-transform: none; /* เพื่อไม่ให้ตัวอักษรเป็นตัวพิมพ์ใหญ่ทั้งหมด */
}

/* Custom Chip styles */
.custom-chip {
  background-color: #E0E0E0 !important; /* Background color for chips */
  color: #424242 !important; /* Text color for chips */
  border-radius: 8px !important;
  font-weight: 500;
  padding: 0 10px;
}

/* Card styles for Artwork and Info */
.artwork-card, .recent-search-card, .info-card {
  background-color: white !important; /* พื้นหลังสีขาว */
  border: 1px solid #E0E0E0; /* Border สีเทาอ่อน */
}
</style>