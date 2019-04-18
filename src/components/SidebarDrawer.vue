<template>
  <v-navigation-drawer
    v-model="drawer"
    absolute
    temporary
  >
    <v-list class="pt-0">
      <v-list-tile @click.stop="drawer = !drawer">
        <v-list-tile-action />
        <v-list-tile-action />
        <v-list-tile-content>
          <v-icon>fas fa-chevron-left</v-icon>
        </v-list-tile-content>
      </v-list-tile>

      <v-divider light></v-divider>

      <v-list-tile to="/" active-class="active-link">
         <v-list-tile-action>
            <v-icon>fas fa-home</v-icon>
          </v-list-tile-action>
        <v-list-tile-content>
          <v-list-tile-title v-text="'Home'"></v-list-tile-title>
        </v-list-tile-content>
      </v-list-tile>

      <v-list-tile to="/login" active-class="active-link">
        <v-list-tile-action>
            <v-icon>fas fa-sign-in-alt</v-icon>
          </v-list-tile-action>
        <v-list-tile-content>
          <v-list-tile-title v-text="'Login'"></v-list-tile-title>
        </v-list-tile-content>
      </v-list-tile>

      <v-list-tile to="/signup" active-class="active-link">
        <v-list-tile-action>
            <v-icon>fas fa-sign-out-alt</v-icon>
          </v-list-tile-action>
        <v-list-tile-content>
          <v-list-tile-title v-text="'Sign Up'"></v-list-tile-title>
        </v-list-tile-content>
      </v-list-tile>

    </v-list>
  </v-navigation-drawer>
</template>

<script>
export default {
  name: 'sidebar-drawer',
  data() {
    return {
      drawer: false,
      items: ['One','Two','Three']
    }
  },
}
</script>
