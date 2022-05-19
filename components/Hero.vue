<template>
  <div class="hero-gradient h-[100vh] flex flex-col gap-2 pt-[100px]">
    <h1 class="text-[42px] px-[20px] text-center">Deine Job website</h1>
    <div class="hero-image w-[100vw]"></div>
    <div class="hero-svg">
      <svg
        data-name="Layer 1"
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 1200 120"
        preserveAspectRatio="none"
      >
        <path
          d="M321.39,56.44c58-10.79,114.16-30.13,172-41.86,82.39-16.72,168.19-17.73,250.45-.39C823.78,31,906.67,72,985.66,92.83c70.05,18.48,146.53,26.09,214.34,3V0H0V27.35A600.21,600.21,0,0,0,321.39,56.44Z"
          class="shape-fill"
        ></path>
      </svg>
    </div>
  </div>
</template>

<style scoped>
.hero-gradient {
  background: transparent linear-gradient(141deg, #ebf4ff 0%, #e6fffa 100%) 0%
    0% no-repeat padding-box;
}

.hero-image {
  background: transparent url("../assets/images/undraw_agreement_aajr.svg") -10px
    0% no-repeat padding-box;
  height: 404.84px;
}

.hero-svg {
  position: absolute;
  bottom: 0;
  left: 10px;
  width: 100%;
  overflow: hidden;
  line-height: 0;
  transform: rotate(180deg);
}

.hero-svg svg {
  position: relative;
  display: block;
  width: calc(100% + 330px);
  height: 130px;
}

.hero-svg .shape-fill {
  fill: #ffffff;
}
</style>
