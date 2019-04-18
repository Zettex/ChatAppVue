<template>
  <v-toolbar color="primary">
    <v-btn 
        icon 
        class="hidden-md-and-up"
        @click.stop="$emit('toggle-drawer')">
      <v-icon>fas fa-bars</v-icon>
    </v-btn>

    <v-toolbar-title>Chat app</v-toolbar-title>

    <v-spacer></v-spacer>

    <v-toolbar-items class="hidden-sm-and-down">
      <v-btn flat to="/">Home</v-btn>
      <v-btn flat to="/Login">Login</v-btn>
      <v-btn flat to="/SignUp">Sign Up</v-btn>
    </v-toolbar-items>

  </v-toolbar>
</template>

<script>
export default {
  name: 'navbar',
  data() {
    return {
    }
  },
}
</script>
