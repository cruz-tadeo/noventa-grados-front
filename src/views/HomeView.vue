<script lang="ts" setup>
import { io } from "socket.io-client";

const socket = io('http://localhost:3001')

socket.on("connect", () => {
  console.log(socket.id, 'probando'); // x8WIv7-mJelg7on_ALbx
});

socket.emit('message', 'Hola mundo probadno')

</script>
<template>
  <main>
    <h2>Probando el sistem completo</h2>
  </main>
</template>
