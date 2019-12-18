<template>
  <div>
    <div id="nav">
      <router-link
        to="/"
      >
        Home
      </router-link>
      <router-link
        v-if="$auth.isAuthenticated"
        to="/profile"
      >
        | Profile
      </router-link>
    </div>
    <br>
    <router-view />
  </div>
</template>

<script>
export default {
  components: {
  }
}
</script>
