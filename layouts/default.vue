<template>
  <div class="h-[100vh] relative">
    <div class="header fixed top-0 bg-light">
      <div class="nav-gradient h-[5px] w-[100vw]"></div>
      <nav
        class="rounded-b-lg shadow-[0_4px_15px_rgba(0,0,0,0.3)] flex w-[100vw] h-[67px] justify-end items-center p-[17px]"
      >
        <a href="#" class="text-textLight hover:text-bgPrimary">Login</a>
      </nav>
    </div>
    <slot />
    <div class="footer bottom-0 fixed bg-light">
      <nav
        class="rounded-t-lg shadow-[0_-2px_15px_rgba(0,0,0,0.3)] flex w-[100vw] h-[128px] justify-center items-center"
      >
        <button
          class="btn-gradient rounded-[12px] w-[320px] h-[40px] text-light"
        >
          Kostenlos Registrieren
        </button>
      </nav>
    </div>
  </div>
</template>

<style scoped>
.nav-gradient {
  background: transparent linear-gradient(91deg, #319795 0%, #3182ce 100%) 0% 0%
    no-repeat padding-box;
}

.btn-gradient {
  background: transparent linear-gradient(95deg, #319795 0%, #3182ce 100%) 0% 0%
    no-repeat padding-box;
}
</style>
