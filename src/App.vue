<template>
  <div id="app">
    <SocialBar/>
    <NavBar/>
    <router-view/>
  </div>
</template>

<script>
import NavBar from '@/components/NavBar';
import SocialBar from '@/components/SocialBar';

export default {
  name: 'App',
  components: {
    SocialBar,
    NavBar,
  },
};
</script>

<style lang="scss">
@import './src/styles/variables.scss';
body {
  margin: 0;
  color: $green-brown;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  .smallcaps {
    font-variant: small-caps;
  }
  .tight-padding {
    padding-left: 20%;
    padding-right: 20%;
  }
  .black-text {
    color: black;
  }
  p {
    margin: 0px;
  }
  > div {
    padding: 0px 20px;
    &.bot-pad {
      padding: 0px 0px 30px !important;
    }
  }
}
</style>
