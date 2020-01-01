<template>
  <div id="app" class="bg-gray-100 font-sans w-full min-h-screen m-0">
    <div class="bg-white shadow">
      <div class="container mx-auto px-4">
        <div class="flex items-center justify-between py-4">
          <div>
            <img alt="Vue logo" src="@/assets/logo.png" class="w-10 h-10" />
          </div>

          <div class="hidden sm:flex sm:items-center">
            <router-link
              to="/"
              class="text-gray-800 text-sm font-semibold hover:text-purple-600 mr-4"
              >Home</router-link
            >
            <router-link
              to="/about"
              class="text-gray-800 text-sm font-semibold hover:text-purple-600 mr-4"
              >About</router-link
            >
          </div>

          <div class="hidden sm:flex sm:items-center">
            <a
              href="#"
              class="text-gray-800 text-sm font-semibold hover:text-purple-600 mr-4"
              >Sign in</a
            >
            <a
              href="#"
              class="text-gray-800 text-sm font-semibold border px-4 py-2 rounded-lg hover:text-purple-600 hover:border-purple-600"
              >Sign up</a
            >
          </div>
        </div>
      </div>
    </div>
    <router-view />
  </div>
</template>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
