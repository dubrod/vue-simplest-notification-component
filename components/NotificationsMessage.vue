<template>
  <section v-if="msg" class="notifications-list">
    <div class="alert alert-success alert-dismissible fade show" role="alert">
      <button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close" @click="closeNotification()"></button>
      {{ msg }}
    </div>
  </section>
</template>

<script>
export default {
  props: ['msg'],
  methods: {
    closeNotification(){
      this.$root.notifications.msg = ''
    }
  }
}
</script>

<style>
.notifications-list{
  position: fixed;
  right:0;
  top:0;
  margin:1rem 1rem 0 0;
  width: 320px;
}
</style>
