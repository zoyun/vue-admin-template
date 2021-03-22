<template>
  <div>
      <el-menu
        :default-active="activeMenu"
        class="el-menu-demo"
        mode="horizontal"
      >
        <menu-item v-for="route in routes" :key="route.path" :item="route" :base-path="route.path" />
      </el-menu>
  </div>
</template>

<script>

import Logo from './Logo'
import MenuItem from './MenuItem'
import variables from '@/styles/variables.scss'

export default {
  components: { MenuItem, Logo },
  computed: {

    routes() {
      return this.$router.options.routes
    },
    activeMenu() {
      const route = this.$route
      const { meta, path } = route
      // if set path, the sidebar will highlight the path you set
      if (meta.activeMenu) {
        return meta.activeMenu
      }
      return path
    },
    showLogo() {
      return this.$store.state.settings.sidebarLogo
    },
    variables() {
      return variables
    },
  }
}
</script>
