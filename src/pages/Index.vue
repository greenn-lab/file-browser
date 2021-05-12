<template>
  <q-page class="q-px-md">
    <h1>File Browser</h1>

    <div class="row">
      <q-card-section class="col-4 file-browser__tree">
        <q-list bordered class="rounded-borders">
          <q-expansion-item
            default-opened
            expand-separator
            icon="folder"
            label="Folders"
          />

          <q-expansion-item
            caption="7 items"
            default-opened
            expand-separator
            expand-icon="off"
            icon="schedule"
            label="Recently"
            @click="select($event)"
          />
        </q-list>
      </q-card-section>
      <q-card-section class="col-8">123</q-card-section>

      <div class="col-12 justify-end">
        <q-btn color="secondary" flat>CLOSE</q-btn>
      </div>
    </div>
  </q-page>
</template>

<script setup>

const select = (e) => {
  console.log('check #1', e.target)
}

</script>

<style lang="scss" scoped>
h1 {
  font-size: 2rem;
}
</style>
