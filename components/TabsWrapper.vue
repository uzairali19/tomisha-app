<script setup>
import { useSlots, ref, provide } from "vue";
const slots = useSlots();
const tabTitles = ref(slots.default().map((tab) => tab.props.title));
const selectedTitle = ref(tabTitles.value[0]);
provide("selectedTitle", selectedTitle);
</script>

<template>
  <div class="mt-[27px] relative mb-[200px]">
    <ul
      class="tabs__header flex absolute top-0 left-[20px]"
      :class="{
        active: selectedTitle === 'Arbeitgeber',
        active2: selectedTitle === 'Temporärbüro',
      }"
    >
      <li
        v-for="title in tabTitles"
        :key="title"
        class="w-[160px] h-[40px] border border-borderPrimary border-solid flex justify-center items-center tabs__item bg-light"
        :class="{
          selected: selectedTitle === title && title === 'Arbeitnehmer',
          secondSelected: selectedTitle === title && title === 'Arbeitgeber',
          thirdSelected: selectedTitle === title && title === 'Temporärbüro',
        }"
        @click="
          (e) => {
            e.preventDefault();
            selectedTitle = title;
          }
        "
      >
        {{ title }}
      </li>
    </ul>

    <slot />
  </div>
</template>

<style scoped>
.tabs__header {
  width: calc(160px * 3);
}
.tabs__header.active {
  left: -40px;
  width: calc(160px * 5);
}

.tabs__header.active2 {
  left: -140px;
  width: calc(160px * 7);
}
.tabs__item.selected {
  background-color: #81e6d9;
  color: #fff;
  transition: 0.3s;
  border-radius: 12px 0px 0px 12px;
}

.tabs__item.secondSelected {
  background-color: #81e6d9;
  color: #fff;
  transition: 0.3s;
}

.tabs__item.thirdSelected {
  background-color: #81e6d9;
  color: #fff;
  transition: 0.3s;
  border-radius: 0px 12px 12px 0px;
}
</style>
