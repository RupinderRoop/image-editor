<template>
  <div class="footer">
    <div class="container">
      <div class="row py-4">
        <div class="col-md-6 py-3">
          <img class="logo-image" src="../../../public/logo_no_text.png" alt="logo">
          <div>&copy; by Inkoop</div>
        </div>
        <div class="col-md-6 text-right py-4">
          <div>4th Floor, #164,</div>
          <div>9th Main Rd, Sector 6,</div>
          <div>HSR Layout, Bengaluru,</div>
          <div>Karnataka 560102</div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
$primary-color:  #00b782;
$secondary-color: #fff;

.footer {
  background-color: $primary-color;
  color: $secondary-color;
}
.logo-image {
  height: 100px;
  width: 120px;
}
</style>
