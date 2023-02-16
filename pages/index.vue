<template lang="pug">
NConfigProvider
  NMessageProvider
    NNotificationProvider
      h1 input form
      ProvideData
</template>

<script lang="ts" setup>
import {
  NConfigProvider,
  NMessageProvider,
  NNotificationProvider,
} from 'naive-ui'
// @ts-ignore
import ProvideData from '../components/ProvideData.vue'



</script>

<style>
body {
  padding: 16px;
}
</style>
