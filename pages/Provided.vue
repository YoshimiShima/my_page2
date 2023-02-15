<template>
  <NSpace>
    <NButton @click="cb1">send</NButton>
  </NSpace>
</template>

<script lang="ts" setup>
import {
  useMessage,
  useNotification,
  useDialog,
  useLoadingBar,
  NButton,
  NSpace
} from 'naive-ui'

const message = useMessage()
const notification = useNotification()
const dialog = useDialog()
const loadingBar = useLoadingBar()

const cb1 = () => {
  message.info('successfully sent')
}

</script>
