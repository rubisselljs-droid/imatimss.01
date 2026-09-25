<script setup>
import { ref } from 'vue'
import { FlLaptopPerson } from '@kalimahapps/vue-icons';

</script>

<template>
   <div class="flex   border-2 border-sky-950 rounded-lg font-sans w-2xs">
      <div>
         <h1 class="text-neutral font-bold">TOTAL DE REGISTROS</h1>
         <span class="flex justify-center items-center border-neutral border-2 w-10 h-10"><FlLaptopPerson/></span>
      </div>
      <div class="flex">
        <span class="font-bold">1,000</span> 
      </div>
     
   </div>
</template>
