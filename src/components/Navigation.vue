<template>
  <section class="nav">
    <div class="text-center">
      <router-link v-if="page !== 'home'" to="/">[ HOME ]</router-link>
      <router-link v-if="page !== 'investments'" to="/investments">[ INVESTMENTS ]</router-link>
      <router-link v-if="page !== 'news'" to="/news">[ NEWS ]</router-link>
      <router-link v-if="page !== 'bootcamps'" to="/bootcamps">[ BOOTCAMPS ]</router-link>
      <router-link v-if="page !== 'podcasts'" to="/podcasts">[ PODCAST ]</router-link>
      <router-link v-if="page !== 'advisors' && page !== 'team'" to="/team">[ TEAM ]</router-link>
    </div>
  </section>
</template>

<script>

export default {
  name: 'Navigation',
  props: ['page'],
  data() {
    return {
    };
  },
};

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.nav {
  font-family: 'Nixie One', "Helvetica Neue";
  margin-bottom: 10px;
  justify-content: center;
  margin-top: 20px;
}

 @media only screen
  and (min-device-width : 320px)
  and (max-device-width : 568px)
  and (orientation : portrait) {

    .nav {
      height: 60px; /* handle 2 lines of nav on mobile*/
    }
}

a, a:hover {
  white-space: nowrap;
  text-decoration: none;
}

a:hover {
  color: darkblue;
}
</style>
