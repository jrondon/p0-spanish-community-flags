<template>
  <SpanishCommunityFlags class="flag" isoCode="AN" />
  <SpanishCommunityFlags class="flag" isoCode="AR" />
  <SpanishCommunityFlags class="flag" isoCode="AS" />
  <SpanishCommunityFlags class="flag" isoCode="IB" />
  <SpanishCommunityFlags class="flag" isoCode="CN" />
  <SpanishCommunityFlags class="flag" isoCode="CB" />
  <SpanishCommunityFlags class="flag" isoCode="CM" />
  <SpanishCommunityFlags class="flag" isoCode="CL" />
  <SpanishCommunityFlags class="flag" isoCode="CT" />
  <SpanishCommunityFlags class="flag" isoCode="EX" />
  <SpanishCommunityFlags class="flag" isoCode="GA" />
  <SpanishCommunityFlags class="flag" isoCode="MD" />
  <SpanishCommunityFlags class="flag" isoCode="MC" />
  <SpanishCommunityFlags class="flag" isoCode="NC" />
  <SpanishCommunityFlags class="flag" isoCode="PV" />
  <SpanishCommunityFlags class="flag" isoCode="RI" />
  <SpanishCommunityFlags class="flag" isoCode="VC" />
</template>

<script>
import SpanishCommunityFlags from "./components/SpanishCommunityFlags.vue";

export default {
  name: "App",
  components: {
    SpanishCommunityFlags,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.flag {
  width: 50px;
  margin: 10px;
}
</style>
