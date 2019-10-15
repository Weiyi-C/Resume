<template>
  <div>
    <b-navbar toggleabale="lg" type="dark" variant="success">
      <b-container>
        <b-navbar-brand href="#">
          <b-img :src=logoSrc fluid alt="郑维一 logo">郑维一 logo</b-img>
          郑维一
        </b-navbar-brand>
        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
        <b-collapse id="nav-collapse" is-nav>
          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto">
            <b-nav-item-dropdown right>
              <!-- Using 'button-content' slot -->
              <template slot="button-content"><em>User</em></template>
              <b-dropdown-item href="#">Profile</b-dropdown-item>
              <b-dropdown-item href="#">Sign out</b-dropdown-item>
            </b-nav-item-dropdown>
          </b-navbar-nav>
        </b-collapse>
      </b-container>
    </b-navbar>
  </div>
</template>

<script>
export default {
  data () {
    return {
      meal: '',
      logoSrc: require('../assets/logo.svg')
    }
  },
  methods: {
    getMeal () {
    }
  }
}
</script>
