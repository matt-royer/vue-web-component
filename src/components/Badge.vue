<template>
  <div :class="classes" data-test="badge">
    <icon :name="$props.icon" v-if="!!$props.icon" />
    <span class="text" data-test="text" v-if="!!$props.text">{{ $props.text }}</span>
  </div>
</template>

<script lang="ts">
import Vue from 'vue';
import Icon from './Icon.vue';

export default Vue.extend({
  components: {
    Icon,
  },
  props: {
    icon: {
      type: String,
      required: false,
      default: null,
    },
    text: {
      type: String,
      required: false,
      default: ""
    },
    small: {
      type: Boolean,
      default: false
    },
    large: {
      type: Boolean,
      default: false
    },
    xl: {
      type: Boolean,
      default: false
    },
    type: {
      type: String,
      required: false,
      default: "default",
    },
  },
  computed: {
    classes(): string[] {
      return [
        "badge",
        this.type,
        !!this.icon && !this.text ? "icon-only" : "",
        this.small ? "small" : "",
        this.large ? "large" : "",
        this.xl ? "xl" : "",
      ];
    }
  },
});
</script>

<style lang="less" scoped>
.variant() {
  padding: @spacing @spacing * 1.5;
  border-radius: @border-radius;
  font-size: @font-size;
  line-height: @font-size;

  .icon {
    height: @font-size;
    line-height: @font-size;
    margin-right: @spacing;

    img {
      height: @icon-size;
      width: @icon-size;
    }
  }
}

.badge {
  @font-size: 0.75rem;
  @spacing: 0.5rem;
  @border-radius: 2.5rem;
  @icon-size: 1rem;

  color: #000000;
  background-color: #ffffff;
  display: inline-block;
  font-weight: 500;
  display: inline-flex;
  align-items: center;
  vertical-align: top;
  user-select: none;
  .variant();

  .icon {
    display: inline-flex;
    align-items: center;

    img {
      margin: 0;
      display: block;
      pointer-events: none;
    }
  }

  &.primary {
    background-color: #DA374A;
    color: #ffffff;
  }
  &.secondary {
    background-color: #162C68;
    color: #ffffff;
  }
  &.accent {
    background-color: #4A5A8C;
    color: #ffffff;
  }
  &.light {
    background-color: rgba(255, 255, 255, 0.8);
  }
  &.dark {
    background-color: rgba(0, 0, 0, 0.8);
    color: #ffffff;
  }
  &.highlight {
    background-color: #F0F600;
  }
  &.featured {
    background-color: #7F8AB0;
    color: #ffffff;
  }

  &.small {
    @spacing: 0.25rem;
    @border-radius: 0.25rem;
    .variant();
  }
  &.large {
    @font-size: 1rem;
    @spacing: 0.5rem;
    @icon-size: 1.25rem;
    .variant();
  }
  &.xl {
    @font-size: 1.25rem;
    @spacing: 0.5rem;
    @icon-size: 1.25rem;
    .variant();
  }

  &.icon-only .icon {
    display: flex;
    margin-right: 0;
  }
}
</style>