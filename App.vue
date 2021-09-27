<template>
  ...
  <NotificationsMessage :msg="notifications.msg" />
</template>

<script>
import NotificationsMessage from '@/components/NotificationsMessage.vue'

export default {
  data() {
    return {
      notifications: {
        msg: ''
      }
    }
  },
  components: {
    NotificationsMessage
  }
}
</script>
