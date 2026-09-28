<template>
  <div class="flex flex-wrap gap-4 p-4">
    <div
      v-for="(dato, index) in datos"
      :key="index"
      class="shadow-sm rounded-2xl font-sans w-2xs bg-white p-5"
    >
     
      <div class="flex justify-between items-start mb-6">
        <h1 class="text-neutral-500 text-xs font-bold tracking-wider uppercase pt-2">
          {{ dato.titulo }}
        </h1>
        <span class="flex justify-center items-center bg-gray-100 rounded-lg p-2">
          <FlLaptopPerson class="w-6 h-6 text-emerald-900" />
        </span>
      </div>

      <!-- Número principal -->
      <div class="mb-4">
        <span class="text-5xl font-bold text-neutral-900 tracking-tight">
          {{ dato.total.toLocaleString() }}
        </span>
      </div>

      <!-- Cobertura + Inventario -->
      <div class="flex items-start gap-4">
        <div class="flex flex-col">
          <span class="text-emerald-800 font-bold text-lg leading-tight">
            {{ dato.cobertura }}%
          </span>
          <span class="text-emerald-800 font-bold text-sm leading-tight">
            Cobertura
          </span>
        </div>

        <div class="flex items-start text-neutral-500 text-sm leading-snug pt-0.5">
          <span class="mr-2">·</span>
          <span>Inventario<br />nacional</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const datos = [
  { titulo: 'Total Registrados',   total: 1325, cobertura: 100 },
  { titulo: 'Activos en línea',    total: 1000, cobertura: 100 },
  { titulo: 'Inactivos / reposo',  total: 64,   cobertura: 100 },
  { titulo: 'Sin nada que hacer solo un chico tranquilo',         total: 13,   cobertura: 100 },
   { titulo: 'Inactivos / reposo',  total: 64,   cobertura: 100 },
]
</script>