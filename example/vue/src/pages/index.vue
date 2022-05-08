<script setup lang="ts">
import unoButton from '@unoui/button'

function go(){
  console.log("button")
}


</script>

<template>
  <div>
    <unoButton type="success" @click="go" name="Success" />
    <br />
    <unoButton type="warning" @click="go" name="Warning" />
    <br />
    <unoButton type="error" @click="go" name="Error" />
    <br />
    <unoButton type="info" @click="go" name="Info" />
    <br />
    <unoButton @click="go" name="Basic" />
  </div>
</template>
