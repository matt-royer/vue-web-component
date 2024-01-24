<template>
  <div id="app">
    <label>Figma References</label>
    <a href="https://www.figma.com/file/4tCQJlwEpKBUOOYT5ijqQL/%F0%9F%93%BD%EF%B8%8F---Design-System?node-id=11331%3A262343" target="_blank">Badge</a>
    <br />
    <a href="https://www.figma.com/file/WrIjx9VD2ohV1SW0b4ByID/Event-Cards?node-id=863%3A2474&mode=dev" target="_blank">Status Badge</a>
    <br /><br />

    <label>Badge (type)</label>
    <badge text="Default" />
    <badge text="Primary" type="primary" />
    <badge text="Secondary" type="secondary" />
    <badge text="Accent" type="accent" />
    <badge text="Light" type="light" />
    <badge text="Dark" type="dark" />
    <badge text="Highlight" type="highlight" />
    <badge text="Featured" type="featured" />
    <br />

    <label>Badge (size)</label>
    <badge text="Small" small />
    <badge text="Default" />
    <badge text="Large" large />
    <badge text="Extra Large" xl />
    <br />

    <label>Badge (icon)</label>
    <badge text="Label" icon="live" small />
    <badge icon="live" small />
    <badge text="Label" icon="live" />
    <badge icon="live" />
    <badge text="Label" icon="live" large />
    <badge icon="live" large />
    <badge text="Label" icon="live" xl />
    <badge icon="live" xl />
    <br />

    <label>Example Status Badges</label>
    <badge text="Live" icon="live" type="primary" />
    <badge text="Postponed" icon="cancel" type="primary" />
    <badge text="Upcoming" icon="calendar" type="accent" />
    <badge text="On Demand" icon="list" />
    <badge text="Highlight" icon="camera" type="highlight" />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Badge from './components/Badge.vue'

export default Vue.extend({
  name: 'App',
  components: {
    Badge
  }
});
</script>

<style lang="less">
@import url('https://fonts.googleapis.com/css?family=Montserrat:300,400,500,600,700,800');

body {
  font-family: "Montserrat", "Open Sans", "calibri", "arial", sans-serif;
  background-color: #09121a;
  color: #fff;
  margin: 1.5rem;
}

#app {
  label {
    font-weight: 500;
    font-size: 0.75rem;
    display: block;
    margin: 1rem 0 0.75rem;
  }

  & > * {
    margin-bottom: 0.25rem;
    margin-right: 0.25rem;
  }

  a {
    color: #0e75d2;
    font-size: 0.75rem;
    font-weight: 800;
    text-transform: uppercase;
    text-decoration: none;

    &:hover {
      text-decoration: underline;
    }
  }
}
</style>
