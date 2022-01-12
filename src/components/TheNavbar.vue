<template>
  <nav id="nav">
    <div class="nav-content">
      <RouterLink to="/">
        <i class="bx bx-home bx-sm"></i>
      </RouterLink>
      <RouterLink to="/store">
        <i class="bx bx-store-alt bx-sm"></i>
      </RouterLink>
      <RouterLink to="/favorites">
        <i class="bx bx-heart bx-sm"></i>
      </RouterLink>
      <RouterLink to="/history">
        <i class="bx bx-history bx-sm"></i>
      </RouterLink>
    </div>
  </nav>
</template>
<style>
#nav {
  width: 100%;
  position: fixed;
  bottom: 0;
  background-color: #fff;
  box-shadow: 0px 0px 2.6px rgb(0 0 0 / 4%), 0px 0px 21px rgb(0 0 0 / 8%);
}
.nav-content {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 20px 25px;
}
.nav-content a.router-link-active i {
  color: rgb(255, 131, 62);
}
</style>
