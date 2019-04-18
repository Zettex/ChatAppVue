<template>
  <v-app dark>

    <navbar
      @toggle-drawer="$refs.drawer.drawer = !$refs.drawer.drawer" />
    
    <sidebar-drawer 
      ref="drawer" />

    <v-content>
      <router-view />
    </v-content>

  </v-app>
</template>

<script>
import Navbar from './components/Navbar';
import SidebarDrawer from './components/SidebarDrawer';

export default {
  name: 'app',
  components: {
    Navbar,
    SidebarDrawer,
  },
  data() {
    return {
    }
  },
}
</script>

<style>
.v-icon{
  font-size: 18px !important;
}

.v-list__tile__content {
  font-size: 16px;
}

.active-link {
  background-color: #1976d2;
}
</style>
