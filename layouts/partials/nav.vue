<template>
  <nav 
    class="navbar" 
    role="navigation" 
    aria-label="main navigation">

    <div class="navbar-brand">
      <a 
        class="navbar-item" 
        href="https://bulma.io">
        <img 
          src="https://bulma.io/images/bulma-logo.png" 
          width="112" 
          height="28">
      </a>

      <a 
        role="button" 
        class="navbar-burger burger" 
        aria-label="menu" 
        aria-expanded="false" 
        data-target="navbarBasicExample">
        <span aria-hidden="true"/>
        <span aria-hidden="true"/>
        <span aria-hidden="true"/>
      </a>
    </div>
    <!-- /.navbar-brand -->

    <div 
      id="navbarBasicExample" 
      class="navbar-menu">

      <div class="navbar-start">
        <a class="navbar-item">
          Home
        </a>

        <a class="navbar-item">
          Documentation
        </a>

        <div class="navbar-item has-dropdown is-hoverable">
          <a class="navbar-link">
            More
          </a>

          <div class="navbar-dropdown">
            <a class="navbar-item">
              About
            </a>
            <a class="navbar-item">
              Jobs
            </a>
            <a class="navbar-item">
              Contact
            </a>
            <hr class="navbar-divider">
            <a class="navbar-item">
              Report an issue
            </a>
          </div>
          
        </div>
      </div>
      <!-- /.navbar-start -->


      <div class="navbar-end">
        <div class="navbar-item">
          <div class="buttons">
            <a class="button is-crfBlue">
              <strong>Parent Login</strong>
            </a>
            <a class="button is-primary is-outlined">
              <CabinSvg class="test" />Latest Newsletter
            </a>
          </div>
        </div>
      </div>
    </div>
    <!-- /.navbar-end -->
  </nav>
</template>

<script>
import CabinSvg from '@/assets/svg/cabin.svg'

export default {
  name: 'Nav',
  components: {
    CabinSvg
  }
}
</script>

<style lang="scss">
.test {
  width: 35px;
  height: 28px;
  margin-right: 10px;
  fill: $crfRed;
}
</style>
