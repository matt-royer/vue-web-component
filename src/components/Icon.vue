<template>
  <span class="icon" data-test="icon">
    <template v-if="$props.name === 'calendar'">
      <svg width="14" height="14" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg">
        <g id="calendar_today" clip-path="url(#clip0_1315_2761)">
          <path id="Vector" d="M11.6667 1.74998H11.0834V0.583313H9.91675V1.74998H4.08341V0.583313H2.91675V1.74998H2.33341C1.69175 1.74998 1.16675 2.27498 1.16675 2.91665V12.25C1.16675 12.8916 1.69175 13.4166 2.33341 13.4166H11.6667C12.3084 13.4166 12.8334 12.8916 12.8334 12.25V2.91665C12.8334 2.27498 12.3084 1.74998 11.6667 1.74998ZM11.6667 12.25H2.33341V4.66665H11.6667V12.25Z" fill="currentColor"/>
        </g>
        <defs>
          <clipPath id="clip0_1315_2761">
            <rect width="14" height="14" fill="currentColor"/>
          </clipPath>
        </defs>
      </svg>
    </template>
    <template v-if="$props.name === 'camera'">
      <svg width="14" height="14" viewBox="0 0 14 14" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
        <g id="camera_roll" clip-path="url(#clip0_1315_1262)">
          <path id="Vector" d="M8.16675 2.91665C8.16675 2.27498 7.64175 1.74998 7.00008 1.74998H6.41675V1.16665C6.41675 0.845813 6.15425 0.583313 5.83341 0.583313H3.50008C3.17925 0.583313 2.91675 0.845813 2.91675 1.16665V1.74998H2.33341C1.69175 1.74998 1.16675 2.27498 1.16675 2.91665V11.6666C1.16675 12.3083 1.69175 12.8333 2.33341 12.8333H7.00008C7.64175 12.8333 8.16675 12.3083 8.16675 11.6666H12.8334V2.91665H8.16675ZM7.00008 10.5H5.83341V9.33331H7.00008V10.5ZM7.00008 5.24998H5.83341V4.08331H7.00008V5.24998ZM9.33341 10.5H8.16675V9.33331H9.33341V10.5ZM9.33341 5.24998H8.16675V4.08331H9.33341V5.24998ZM11.6667 10.5H10.5001V9.33331H11.6667V10.5ZM11.6667 5.24998H10.5001V4.08331H11.6667V5.24998Z" fill="currentColor"/>
        </g>
        <defs>
          <clipPath id="clip0_1315_1262">
            <rect width="14" height="14" fill="currentColor"/>
          </clipPath>
        </defs>
      </svg>
    </template>
    <template v-if="$props.name === 'cancel'">
      <svg width="14" height="14" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg">
        <g id="cancel" clip-path="url(#clip0_1315_2560)">
          <path id="Vector" d="M7.00008 1.16669C3.77425 1.16669 1.16675 3.77419 1.16675 7.00002C1.16675 10.2259 3.77425 12.8334 7.00008 12.8334C10.2259 12.8334 12.8334 10.2259 12.8334 7.00002C12.8334 3.77419 10.2259 1.16669 7.00008 1.16669ZM7.00008 11.6667C4.42758 11.6667 2.33341 9.57252 2.33341 7.00002C2.33341 4.42752 4.42758 2.33335 7.00008 2.33335C9.57258 2.33335 11.6667 4.42752 11.6667 7.00002C11.6667 9.57252 9.57258 11.6667 7.00008 11.6667ZM9.09425 4.08335L7.00008 6.17752L4.90591 4.08335L4.08341 4.90585L6.17758 7.00002L4.08341 9.09419L4.90591 9.91669L7.00008 7.82252L9.09425 9.91669L9.91675 9.09419L7.82258 7.00002L9.91675 4.90585L9.09425 4.08335Z" fill="currentColor"/>
        </g>
        <defs>
          <clipPath id="clip0_1315_2560">
            <rect width="14" height="14" fill="currentColor"/>
          </clipPath>
        </defs>
      </svg>
    </template>
    <template v-if="$props.name === 'list'">
      <svg width="14" height="14" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg">
        <g id="list_alt" clip-path="url(#clip0_1315_2565)">
          <path id="Vector" d="M6.41667 4.08333H9.91667V5.25H6.41667V4.08333ZM6.41667 6.41667H9.91667V7.58333H6.41667V6.41667ZM6.41667 8.75H9.91667V9.91667H6.41667V8.75ZM4.08333 4.08333H5.25V5.25H4.08333V4.08333ZM4.08333 6.41667H5.25V7.58333H4.08333V6.41667ZM4.08333 8.75H5.25V9.91667H4.08333V8.75ZM11.725 1.75H2.275C1.98333 1.75 1.75 1.98333 1.75 2.275V11.725C1.75 11.9583 1.98333 12.25 2.275 12.25H11.725C11.9583 12.25 12.25 11.9583 12.25 11.725V2.275C12.25 1.98333 11.9583 1.75 11.725 1.75ZM11.0833 11.0833H2.91667V2.91667H11.0833V11.0833Z" fill="currentColor"/>
        </g>
        <defs>
          <clipPath id="clip0_1315_2565">
            <rect width="14" height="14" fill="currentColor"/>
          </clipPath>
        </defs>
      </svg>
    </template>
    <template v-if="$props.name === 'live'">
      <svg width="14" height="10" viewBox="0 0 14 10" fill="none" xmlns="http://www.w3.org/2000/svg">
        <g id="Group">
          <path id="Vector" d="M5.24992 9.66665C7.82725 9.66665 9.91659 7.57731 9.91659 4.99998C9.91659 2.42265 7.82725 0.333313 5.24992 0.333313C2.67259 0.333313 0.583252 2.42265 0.583252 4.99998C0.583252 7.57731 2.67259 9.66665 5.24992 9.66665Z" fill="currentColor" />
          <path id="Vector_2" d="M9.9165 0.484985V1.70415C11.2757 2.18248 12.2498 3.47748 12.2498 4.99998C12.2498 6.52248 11.2757 7.81748 9.9165 8.29582V9.51498C11.929 8.99582 13.4165 7.17582 13.4165 4.99998C13.4165 2.82415 11.929 1.00415 9.9165 0.484985Z" fill="currentColor" />
        </g>
      </svg>
    </template>
  </span>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
  props: {
    name: {
      type: String,
      required: true,
    },
  },
});
</script>
