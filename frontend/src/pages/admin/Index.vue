<template>
      <div class="admin__container">
        <div class="admin__container-menu-container">
          <ul class="admin__container-menu-container-nav">
            <!-- Links are to sibling routes -->
            <li><router-link to="/admin">View Products</router-link></li>
            <li><router-link to="/admin/new">New Product</router-link></li>
          </ul>
        </div>
        <!-- Outlet for children routes -->
        <router-view class="router__container"></router-view>
      </div>
</template>

<style lang="scss">
.admin__container {
  font-size: 1rem;
  display: flex;
  margin-top: 2rem;
  &-menu-container {
      flex: 0 0 15%;
      border-right: 1px solid #cccccc;
      padding: 2rem;
      &-nav {
          list-style: none;
          & li {
              padding: 1rem 0;
              font-size: 1.2rem;
              & > * {
                  text-decoration: none;
              }
          }
      }
  }
  .router__container {
      flex: 0 0 85%;
  }
}
</style>
