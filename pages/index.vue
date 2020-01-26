<template>
  <div class="container">
    <messages />
    <div class="input-layout">
      <chat-form />
    </div>
  </div>
</template>

<script>
import Messages from "~/components/Messages.vue";
import ChatForm from "~/components/ChatForm.vue";

export default {
  components: {
    Messages,
    ChatForm
  }
};
</script>

<style>
.container {
  height: 100%;
}
.chats-container {
  padding: 16px;
}

.chat-container {
  display: flex;
  padding: 8px;
}

.thumbnail-container {
  margin-right: 16px;
}

.thumbnail-container img {
  width: 50px;
  height: 50px;
  border-radius: 10px;
}

.user-name {
  font-weight: bold;
}
.chats-layout {
  overflow: scroll;
  height: 90%;
}

.input-layout {
  height: 10%;
}
.input-container {
  padding: 10px;
  height: 100%;
}

textarea {
  width: 100%;
  height: 100%;
}
</style>
