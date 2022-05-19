<template>
  <div class="pb-[200px]">
    <div>
      <ul
        class="flex justify-center overflow-x-auto un-ordered-list ml-[20px] mt-10"
      >
        <li>
          <a href="#">Arbeitnehmer</a>
        </li>
        <li><a href="#">Arbeitgeber</a></li>
        <li>
          <a href="#">Temporärbüro</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<style scoped>
.un-ordered-list {
  width: calc(160px * 3);
}
.un-ordered-list li {
  border: 1px solid #cbd5e0;
  width: 160px;
  height: 48px;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
