<template>
  <div class="mb-3">
    <nav class="navbar nav-bg-color justify-content-between">
      <a class="navbar-brand title-text">Image Editor</a>
      <ul class="nav justify-content-end">
        <li class="nav-item">
          <a class="nav-link active" href="#">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">About</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Contact</a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<style lang="scss" scoped>
$primary-color:  #00b782;
$secondary-color: #fff;

.nav-bg-color {
  background-color: $primary-color;
}

a.title-text {
  color: $secondary-color;
}
.nav-link {
  color: $secondary-color
}
</style>
