<template>
  <div :class="classes">
    <span class="icon">
      <img src="@/assets/badge_icons/on_air.svg" draggable="false" v-if="status === 'on_air'" />
      <img src="@/assets/badge_icons/cancel.svg" draggable="false" v-else-if="status === 'postponed'" />
      <img src="@/assets/badge_icons/today.svg" draggable="false" v-else-if="status === 'upcoming'" />
      <img src="@/assets/badge_icons/list.svg" draggable="false" v-else-if="status === 'on_demand'" />
      <img src="@/assets/badge_icons/camera_roll.svg" draggable="false" v-else-if="status === 'highlight'" />
    </span>
    <span class="text">{{text}}</span>
  </div>
</template>

<script>
export default {
  props: {
    status: {
      type: String,
      required: true,
    },
    small: {
      type: Boolean,
      default: false
    },
    large: {
      type: Boolean,
      default: false
    },
  },
  computed: {
    text() {
      return {
        "on_air": "Live",
        "postponed": "Postponed",
        "upcoming": "Upcoming",
        "on_demand": "On Demand",
        "highlight": "Highlight",
      }[this.status];
    },
    classes() {
      return [
        "badge",
        this.status,
        {
          "small": this.small,
          "large": this.large,
        }
      ];
    }
  },
};
</script>

<style lang="less" scoped>
@import url('https://fonts.googleapis.com/css?family=Montserrat:300,400,500,600,700,800');

.badge {
  font-family: "Montserrat", "Open Sans", "calibri", "arial", sans-serif;
  color: #000000;
  background-color: #ffffff;
  display: inline-block;
  padding: 0.5rem 1rem;
  border-radius: 2.5rem;
  font-size: 1rem;
  font-weight: 600;
  display: inline-flex;
  align-items: center;
  vertical-align: top;
  user-select: none;

  .icon {
    margin-right: 0.5rem;

    img {
      margin: 0;
      display: block;
      pointer-events: none;
    }
  }

  &.on_air,
  &.postponed {
    color: #ffffff;
    background-color: #DA374A;
  }
  &.upcoming {
    color: #ffffff;
    background-color: #4A5A8C;
  }
  &.highlight {
    background-color: #F0F600;
  }

  &.small {
    padding: 0.25rem;
    font-size: 0.75rem;
    border-radius: 0.25rem;
    .icon {
      margin-right: 0.25rem;
    }
  }
  &.large {
    padding: 0.75rem 1.25rem;
    font-size: 1.25rem;
    border-radius: 2.5rem;
    .icon img {
      height: 1.25rem;
    }
  }
}
</style>
