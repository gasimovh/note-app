<template>
  <header>
    <div class="container">
      <div class="logo">
        <img src="../assets/logo.png" alt="logo" />
      </div>
      <div class="settings">
        <img src="../assets/gear.png" alt="settings" />
      </div>
    </div>
  </header>
</template>

<script>
export default {};
</script>

<style scoped>
header {
  background-color: #ffffff;
  padding: 10px 25px 10px 25px;
  box-shadow: 0 2px 10px 0 rgba(0, 0, 0, 0.2);
  z-index: 99;
}

.container {
  display: flex;
  justify-content: space-between;
}

img {
  display: block;
  max-width: 100%;
}

.logo {
  width: 40px;
  height: 44px;
}

.settings {
  width: 40px;
  height: 40px;
}
</style>