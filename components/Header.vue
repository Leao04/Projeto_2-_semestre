<template>
  <div>
    <div>
      <b-navbar type="light" variant="dark">
        <b-navbar-nav>
          <NuxtLink to="/">Início</NuxtLink>
          <div class="menu1">
            <NuxtLink to="/">Cine Pipocando</NuxtLink>
          </div>
          <div class="menu2">
            <NuxtLink to="/">Lançamentos</NuxtLink>
          </div>
          <div class="menu3">
            <NuxtLink to="/">Ingressos</NuxtLink>
          </div>
        </b-navbar-nav>
      </b-navbar>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>
