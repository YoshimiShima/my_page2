<template>
  <NConfigProvider inline-theme-disabled>
    <NMessageProvider>
      <NNotificationProvider>
        <NLoadingBarProvider>
          <NDialogProvider>
              NForm
              <NForm
              ref="formRef"
              inline
              :label-width="100"
              :model="formValue"
              :rules="rules"
              :size="size">
                <NFormItem label="FormItem">
                  <NInput />
                </NFormItem>
                <NFormItemRow>
                  
                </NFormItemRow>
              </NForm>
            <Provided />
          </NDialogProvider>
        </NLoadingBarProvider>
      </NNotificationProvider>
    </NMessageProvider>
  </NConfigProvider>
</template>

<script lang="ts" setup>
import {
  NConfigProvider,
  NButton,
  NSpace,
  NA,
  NDialogProvider,
  NForm,
  NFormItem,
  NFormItemCol,
  NFormItemGi,
  NFormItemGridItem,
  NFormItemRow,
  NInput,
  NInputGroup,
  NInputGroupLabel,
  NInputNumber,
  NLoadingBarProvider,
  NMessageProvider,
  NNotificationProvider,
} from 'naive-ui'
import Provided from './Provided.vue'


</script>

<style>
body {
  padding: 16px;
}
</style>
