<template>
  <footer class="footer">
    <div class="footer__logo">
      <img src="../assets/weather-logo.png" alt="logo" class="img__size">
    </div>
    <img src="../assets/footer.jpg" alt="person" class="footer__person">
  </footer>
</template>

<script>
export default {
  name: 'TheFooter'
}
</script>

<style scoped lang="scss">
.footer{
  margin-top:-140px;
  position: relative;
  z-index: -1;
  display:flex;
  justify-content: flex-start;
  align-items: center;
  box-sizing: border-box;
  &__logo{
    position: absolute;
    bottom:5px;
    right:5px;
    @media all and (max-width: 600px){
      position: relative;
      bottom:0;
      right:0;
    }
    img{
      @media all and (max-width: 600px){
        margin-bottom: 15px;
        max-width: 200px;
        height: auto;
      }
    }
  }
  &__person{
    @media all and (max-width: 600px){
      max-width: 100%;
      height: auto;
    }
  }
  @media all and (max-width: 600px){
    flex-direction: column;
    margin-top:-15px;
  }
}
.img__size{
  height: 200px;
  width: 200px;
}
</style>
