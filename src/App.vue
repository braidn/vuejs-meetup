
<template>
  <div class="messages">
    <status></status>
    <messages
      :messages="MessageStore.state.messages"></messages>
    <input-bar
      :store="MessageStore"></input-bar>
  </div>
</template>

<script>
  import InputBar from './components/InputBar.vue'
  import Messages from './components/Messages.vue'
  import Status from './components/Status.js'
  import MessageStore from './store/messages'
  export default {
    data () {
      return {
        MessageStore
      }
    },
    components: {
      InputBar,
      Messages,
      Status
    }
}
</script>

<style> </style>
