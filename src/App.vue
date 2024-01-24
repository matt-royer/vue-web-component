<template>
  <div id="app">
    <PBadge status="on_air" />
    <PBadge status="postponed" />
    <PBadge status="upcoming" />
    <PBadge status="on_demand" />
    <PBadge status="highlight" />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import PBadge from './components/PBadge.vue'

export default Vue.extend({
  name: 'App',
  components: {
    PBadge
  }
});
</script>

<style>
.badge {
  display: block;
}
</style>
