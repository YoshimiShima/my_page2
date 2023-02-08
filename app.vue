<template>
  <n-loading-bar-provider>
    <n-message-provider>
      <n-notification-provider>
        <n-dialog-provider>
          <index />
        </n-dialog-provider>
      </n-notification-provider>
    </n-message-provider>
  </n-loading-bar-provider>
  </template>

  <script>
  import { defineComponent } from "vue";
  import index from "./pages/index.vue";

  export default defineComponent({
  components: {
    index,
  },
  });
  </script>