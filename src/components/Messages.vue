<template>
  <div class="message-history">
    <message v-for="message in messages"
      :message="message">
    </message>
  </div>
</template>

<script>
  import Message from './Message.vue'
  export default {
    props: ['messages'],
    components: {
      Message
    }
  }
</script>

<style></style>
