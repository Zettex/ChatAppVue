<template>
  <v-container fluid fill-height>
    <v-layout align-center justify-center>
      <v-flex xs12 sm8 md4>
        <v-card class="elevation-12">
          <v-toolbar color="primary">
            <v-toolbar-title>SIGN UP FORM</v-toolbar-title>
          </v-toolbar>
          <v-card-text>
            <v-form>
              <v-text-field
                prepend-icon="person"
                name="username"
                label="Username"
                type="text"
                v-model="username"
              >
              </v-text-field>
              <v-text-field
                prepend-icon="email"
                name="email"
                label="Email" 
                type="text"
                v-model="email"
              >
              </v-text-field>
              <v-text-field
                prepend-icon="lock"
                name="password"
                label="Password"
                type="password"
                v-model="password"
              >
              </v-text-field>
              <v-text-field
                prepend-icon="lock"
                name="confirmPassword"
                label="Confirm Password"
                type="password"
                v-model="passwordConfirm"
              >
              </v-text-field>
            </v-form>
          </v-card-text>
          <v-card-actions>
            <v-spacer></v-spacer>
            <v-btn color="primary">Sign Up</v-btn>
          </v-card-actions>
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  data: () => ({
      username: '',
      email: '',
      password: '',
      passwordConfirm: '',
    }),
};
</script>
