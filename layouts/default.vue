<template>
  <div class="flex flex-col justify-between h-[100vh]">
    <div class="header">
      <div class="nav-gradient h-[5px] w-[100vw]"></div>
      <nav
        class="rounded-b-lg shadow-[0_2px_15px_rgba(0,0,0,0.3)] flex w-[100vw] h-[67px] justify-end items-center p-[17px]"
      >
        <a href="#" class="text-textLight hover:text-bgPrimary">Login</a>
      </nav>
    </div>
    <div class="footer">
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
