<template>
  <header class="header">
    <nav class="navbar" role="navigation" aria-label="main navigation">
      <div class="navbar-brand">
        <nuxt-link class="navbar-item" :to="{name:'index'}"><img src="https://bulma.io/images/bulma-logo.png" width="112" height="28"></nuxt-link>
        <div class="navbar-end">
          <div class="navbar-item">
            <div class="buttons">
              <nuxt-link class="button is-primary" :to="{name:'u-join'}"><strong>Join</strong></nuxt-link>
              <!-- <a class="button is-light">Log in</a> -->
            </div>
          </div>
        </div>
      </div>
    </nav>
  </header>
</template>

<script>
export default {
  
}
</script>

<style>
  header{ background-color: red;}
</style>