<template>

  <h2>{{ props.facultad }}</h2>

  <div class="card">
    <DataTable :value="props.semillero" tableStyle="min-width: 50rem">
      <Column field="programa" header="Programa"></Column>
      <Column field="nombre" header="Nombre de semillero"></Column>
      <Column field="grupo" header="Grupo de investigación"></Column>
    </DataTable>
  </div>
</template>

<script setup>
const props = defineProps(
  {
    semillero: Object,
    facultad: String
  }
)
</script>