<template>
  <NForm ref="formRef" :model="model" :rules="rules">
    <NFormItem path="name" label="名前">
      <NInput v-model:value="model.name" @keydown.enter.prevent />
    </NFormItem>
    <NFormItem path="email" label="メールアドレス">
      <NInput v-model:value="model.email" @keydown.enter.prevent />
    </NFormItem>
    <NFormItem path="password" label="パスワード">
      <NInput v-model:value="model.password"
        type="password"
        @input="handlePasswordInput"
        @keydown.enter.prevent />
    </NFormItem>
    <NRow :gutter="[0, 24]">
      <NCol :span="24">
        <div style="display: flex; justify-content: flex-end">
      <NButton @click="handleValidateClick">
        Validate
      </NButton>
        </div>
      </NCol>
    </NRow>
  </NForm>
  <NDatePicker />
</template>

<script lang="ts" setup>
import {
  NForm,
  NFormItem,
  NFormItemCol,
  NFormItemRow,
  NInput,
  NButton,
  NDatePicker,
  FormInst,
  FormItemInst,
  FormItemRule,
  FormValidationError,
  useMessage,
  FormRules,
  NRow,
  NCol
} from 'naive-ui'
import Provided from './Provided.vue'

interface ModelType {
  name: string | null
  password: string | null
  email: string | null
}



</script>

<style>
body {
  padding: 20px;
  width: 800px;
}
</style>