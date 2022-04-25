<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark paddington">
    <NuxtLink class="navbar-brand" to="/">Fire Airbnb</NuxtLink>
    <button
      class="navbar-toggler"
      type="button"
      data-toggle="collapse"
      data-target="#navbarSupportedContent"
      aria-controls="navbarSupportedContent"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
    </button>

    <div id="navbarSupportedContent" class="collapse navbar-collapse ml-auto">
      <ul class="navbar-nav ml-auto">
        <li class="nav-item active">
          <NuxtLink to="/products" class="nav-link"
            >Products <span class="sr-only">(current)</span></NuxtLink
          >
        </li>
        <li class="nav-item active">
          <NuxtLink to="/my-items" class="nav-link"
            >My Items <span class="sr-only">(current)</span></NuxtLink
          >
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {}
</script>

<style lang="css" scoped>
.paddington {
  padding: 1.5rem;
  background-color: black;
}
.nav-left {
  margin-left: auto;
}
</style>
