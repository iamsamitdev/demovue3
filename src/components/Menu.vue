<script setup lang="ts">
</script>

<template>
  <nav class="navbar navbar-expand-lg fixed-top bg-black">
    <div class="container">
      <router-link to="/" class="navbar-brand text-white">Furniture</router-link>
      <button class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse"
        id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <router-link to="/" class="nav-link text-white active"
              aria-current="page">Home</router-link>
          </li>
          <li class="nav-item">
            <router-link to="/about" class="nav-link text-white active"
              aria-current="page">About</router-link>
          </li>
          <li class="nav-item dropdown">
            <a class="nav-link text-white dropdown-toggle"
              href="#"
              role="button"
              data-bs-toggle="dropdown"
              aria-expanded="false">
              Service
            </a>
            <ul class="dropdown-menu">
              <li><a class="dropdown-item"
                  href="#">Menu 1</a></li>
              <li><a class="dropdown-item"
                  href="#">Menu 2</a></li>
              <li>
                <hr class="dropdown-divider">
              </li>
              <li><a class="dropdown-item"
                  href="#">Other menu</a></li>
            </ul>
          </li>
          <li class="nav-item">
            <router-link to="/contact" class="nav-link text-white active"
              aria-current="page">Contact</router-link>
          </li>
        </ul>
        <!-- Login Button -->
        <button class="btn btn-outline-success me-3"
          type="submit">Sign In</button>
        <!-- Register Button -->
        <button class="btn btn-primary"
          type="submit">Sign Up</button>
      </div>
    </div>
  </nav>
</template>

<style scoped></style>