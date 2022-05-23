<script setup lang="ts">
  import tabs from '@/assets/data/tab-data.json'
</script>
<template>
  <div class="body h-[100%]">
    <Hero />
    <TabsWrapper>
      <TabItem :title="tabs[0].title">Content from Tab 1</TabItem>
      <TabItem :title="tabs[1].title"
        >Content from Tab 2 Lorem ipsum dolor sit amet.</TabItem
      >
      <TabItem :title="tabs[2].title"
        ></TabItem
      >
    </TabsWrapper>
  </div>
</template>
