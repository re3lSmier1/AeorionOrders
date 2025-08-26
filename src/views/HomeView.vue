<script setup lang="ts">
  import {ref} from "vue";

  const categories = ref([
    { name: "Sandwiches", image: "/sandwiches.jpg", url: "/sandwiches" },
    { name: "Quesadilla", image: "/quesadilla.png", url: "/quesadilla" },
    { name: "Burgers", image: "/burgers.png", url: "/burgers" },
    { name: "Drinks", image: "/drinks.webp", url: "/drinks" },
    { name: "Fruits", image: "/fruits.jpg", url: "/fruits" },
    { name: "Snacks", image: "/snacks.png", url: "/snacks" },
  ])
</script>

<template>
  <main >
    <nav class="navbar fixed-top bg-body-tertiary">
      <div class="container-fluid">
        <a class="navbar-brand" href="#">Aeorion Orders</a>
        <router-link to="/cart" class="btn btn-link text-decoration-none text-black" style="padding-right: 15px"><i class="bi bi-cart3" style="font-size: 20px"></i> Cart</router-link>
      </div>
    </nav>
    <div class="row" style="width: 100vw; height: calc(100vh - 60px); margin-top: 60px">
      <div class="col-md-3 col-lg-3">
        <div style="display: flex; align-items: center; height: 100vh">
          <ul class="nav flex-column">
            <li class="nav-item" v-for="category in categories">
              <router-link class="nav-link" aria-current="page" :to="category.url">
                <img :src="category.image" alt=""
                     style="max-width: 40px; max-height: 40px; width: auto; height: auto" />
                {{ category.name }}
              </router-link>
            </li>
          </ul>
        </div>
      </div>
      <div class="col-md-9 col-lg-9">
        <div style="padding: 15px">
          <RouterView />
        </div>
      </div>
    </div>
  </main>
</template>

<style scoped>
.nav-item{
  font-size: x-large;
  border-bottom: #ccc 1px solid;
}
.nav-link{
  color: #222222;
}
</style>
