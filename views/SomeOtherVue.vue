<template>
  ...
  <button v-on:click="showNote(value)">Button with a purpose</button>
</template>

<script>
export default {
  methods: {
    showNote(value){
        this.$root.notifications = {
          msg: 'Are you sure you want to delete ' + value
        }
    }
  }
}
</script>
