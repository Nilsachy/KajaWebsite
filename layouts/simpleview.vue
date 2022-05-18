<template>
  <v-app>
    <v-main>
      <v-btn x-large class="icon" icon href="https://www.linkedin.com/in/kaja-wiewi%C3%B3ra-3b52861b6/" target="_blank">
        <v-icon>mdi-linkedin</v-icon>
      </v-btn>
      <v-btn x-large class="icon" icon href="mailto:kaja.wiewiora@gmail.com">
        <v-icon>mdi-email-outline</v-icon>
      </v-btn>
      <v-dialog
        v-model="dialog"
        width="500"
      >
        <template #activator="{ on, attrs }">
          <v-btn
            x-large
            class="icon"
            icon
            v-bind="attrs"
            v-on="on"
          >
            <v-icon>mdi-phone</v-icon>
          </v-btn>
        </template>

        <v-card
          class="pa-5"
        >
          <v-card-title>
            +48 (0)6.97.60.35.47
          </v-card-title>
        </v-card>
      </v-dialog>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      dialog: false
    }
  }
}
</script>

<style>

.icon {
  position: relative;
  left: 15px;
  top:15px;
}

</style>
