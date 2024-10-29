<template>
  <div class="default-layout"> 
    <header class="header-orange">
      <div class="header-top">
        <UContainer class="header-top-coontainer">
          <UButton variant="link" color="white" :padded="false" class="px-3">Daftar</UButton>
          <UButton variant="link" color="white" :padded="false" class="px-3">Login</UButton>
        </UContainer>
      </div>
      <div class="header-bottom">
        <UContainer class="header-bottom-container">
          <BaseLogo />
          <LayoutsSearchBar class="flex-1" />
          <UButton variant="link">
            <IconCart />
          </UButton>
        </UContainer>
      </div>
    </header>
    <main class="main-layout"><slot /></main>
    <footer>Footer</footer>
  </div>
</template>

<style lang="scss" scoped>
  .default-layout {
    @apply flex flex-col;
    @apply min-h-screen;
    @apply bg-red-200;

    .header-orange {
      @apply text-white;
      @apply flex flex-col;
      @apply h-32;

      .header-top {
        @apply bg-primary;
        @apply py-2;

        .header-top-coontainer {
          @apply flex justify-end;
          @apply divide-x divide-gray-50/50;
        }
      }

      .header-bottom {
        @apply bg-gradient-to-b from-primary to-[#FF6633];
        @apply flex-1;

        .header-bottom-container {
          @apply flex justify-between items-center;
          @apply h-full;
          @apply gap-12;
        }
      }
    }

    .main-layout {
      @apply flex-1;
      @apply bg-blue-300;
    }
  }

  
</style>