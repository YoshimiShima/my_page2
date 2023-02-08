<template>
  <NForm>
    <NFormItem label="入力フォーム">
      <NInput />
    </NFormItem>
  </NForm>
  <NFormItemRow>
    <NFormItemCol label="NFormItemCol" span="12">
      <NInput />
    </NFormItemCol>
  </NFormItemRow>
  <NButton type="primary">submit</NButton>
</template>

<script lang="ts" setup>
import {
  NForm,
  NFormItem,
  NFormItemCol,
  NFormItemRow,
  NInput,
  NButton
} from 'naive-ui'
import Provided from './Provided.vue'
</script>

<style>
body {
  padding: 16px;
}
</style>