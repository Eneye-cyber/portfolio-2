<script setup lang="ts">
import Button from '../Button.vue';

</script>

<template>
  <div class="header">
    <div class="header_container">
      <div class="logo"><a href="#"><img src="img/LOGO.png" alt="N_EYE"></a></div>

      <div class="navigation">
        <ul class="navigation_links">
          <li class="navigation_links_container"><a class="link" href="#">Home</a></li>
          <li class="navigation_links_container"><a class="link" href="#">Services</a></li>
          <li class="navigation_links_container"><a class="link" href="#">Templates</a></li>
          <li class="navigation_links_container"><a class="link" href="#">About Us</a></li>
        </ul>
        <Button :secondary=true >Login</Button>
        <Button>Get A Website</Button>

      </div>
    </div>
  </div>
</template>

<style scoped>
.header{
  position: sticky;
  top: 0;
  width: 100%;
  max-height: 81px;
  overflow: hidden;
  box-shadow: 0px 3px 4px rgba(237, 242, 241, 0.8);
  padding: 12px 32px;
}
.header_container{
  margin: 0 auto;
  display: flex;
  align-items: center;
}
.navigation{
  margin-left: auto;
  display: flex;
  align-items: center;
}
.navigation_links{
  display: flex;
  align-items: center;
  gap: 10px;
  margin: 0;
}
.navigation_links_container{
  list-style: none;
}
.navigation_links_container .link{
  display: inline-flex;
  align-items: center;
  justify-content: center;
  text-decoration: none;
  color: #1C4E59;
  font-weight: 500;
  padding: 12px 16px;
}
</style>
