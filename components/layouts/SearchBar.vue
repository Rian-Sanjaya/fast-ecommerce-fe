<template>
  <div class="searchbar">
    <input placeholder="Cek: Flash Sale Rp17 Local!">
    <UButton icon="heroicons:magnifying-glass" class="px-6" />
  </div>
</template>

<style lang="scss" scoped>
.searchbar {
  @apply bg-white;
  @apply p-1;
  @apply flex justify-between items-center gap-2;
  @apply rounded-sm;
  @apply text-black;

  input {
    @apply outline-none pl-3;
    @apply flex-1;
  }
}
</style>