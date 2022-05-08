<script setup lang="ts">

const props = defineProps(['name','type'])

function typeStyle(type:string):string{
  switch(type){
    case 'success':
      return 'bg-emerald-600  hover:bg-emerald-500'
    case 'warning':
      return 'bg-yellow-600  hover:bg-yellow-500'
    case 'error':
      return 'bg-red-600  hover:bg-red-500'
    case 'info':
      return 'bg-blue-600  hover:bg-blue-500'
    default:
      return 'bg-blue-600  hover:bg-blue-500'
  }
}
</script>

<template>
  <div >
    <button
      class="
       px-4 py-2 font-medium tracking-wide transform
       text-white transition-colors duration-200 rounded-md
       focus:outline-none focus:ring focus:ring-blue-300 focus:ring-opacity-80"
      :class="typeStyle(type)">
        {{props.name}}
    </button>
  </div>
</template>
