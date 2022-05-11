<script setup lang="ts">
import {unoGrid} from 'uno-ui'

function go(){
  console.log("button")
}


</script>

<template>
  <div>
    <unoGrid>
      <div class="col-span-1 bg-red-700 ">1</div>
      <div class="col-span-1 bg-blue-700 ">2</div>
      <div class="col-span-1 bg-red-700">3</div>
      <div class=" col-span-2 col-span-1 bg-blue-700">4</div>
      <div class="col-span-1 bg-red-700">5</div>
      <div class="col-span-1 bg-blue-700">6</div>
      <div class="col-span-1 bg-red-700">7</div>
      <div class="col-span-1 bg-blue-700">8</div>
      <div class="col-span-1 bg-red-700">9</div>
    </unoGrid>
  </div>
</template>
