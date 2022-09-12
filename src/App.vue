<script setup>
import { useDark, useToggle } from '@vueuse/core';

const isDark = useDark()
const toggleDark = useToggle(isDark)
</script>

<template>
  <main px-16 py-40 text-center>
    <i i-logos-unocss text-48 inline-block />
    <p mt-15 text-20 font-bold color-gray-400>UnoCSS 指北</p>

    <p text-16 mt-15 inline-flex gap-10>
      <i @click="toggleDark()" icon-btn dark:i-carbon-moon i-carbon-sun />
      <a
        icon-btn i-carbon-logo-github
        href="https://github.com/zclzone"
        target="_blank"
        title="GitHub"
      />
    </p>

    <section mt-20 w-360 mx-auto flex flex-wrap justify-around p-10 card-shadow rounded-10 dark:b >
      <div w-50 h-50 b-1 rounded-5 f-c-c p-10 m-20>
        <span w-6 h-6 rounded-3 bg-black dark:bg-white />
      </div>
      <div w-50 h-50 b-1 rounded-5 flex justify-between p-10 m-20>
        <span w-6 h-6 rounded-3 bg-black dark:bg-white />
        <span w-6 h-6 rounded-3 self-end bg-black dark:bg-white />
      </div>
      <div w-50 h-50 b-1 rounded-5 flex justify-between p-10 m-20>
        <span w-6 h-6 rounded-3 bg-black dark:bg-white />
        <span w-6 h-6 rounded-3 self-center bg-black dark:bg-white />
        <span w-6 h-6 rounded-3 self-end bg-black dark:bg-white />
      </div>
      <div w-50 h-50 b-1 rounded-5 flex justify-between p-10 m-20>
        <div flex-col justify-between>
          <span w-6 h-6 rounded-3 bg-black dark:bg-white />
          <span w-6 h-6 rounded-3 bg-black dark:bg-white />
        </div>
        <div flex-col justify-between>
          <span w-6 h-6 rounded-3 bg-black dark:bg-white />
          <span w-6 h-6 rounded-3 bg-black dark:bg-white />
        </div>
      </div>
      <div w-50 h-50 b-1 rounded-5 flex-col justify-between items-center p-10 m-20>
        <div flex w-full justify-between>
          <span w-6 h-6 rounded-3 bg-black dark:bg-white />
          <span w-6 h-6 rounded-3 bg-black dark:bg-white />
        </div>
        <div w-6 h-6 rounded-3 bg-black dark:bg-white />
        <div flex w-full justify-between>
          <span w-6 h-6 rounded-3 bg-black dark:bg-white />
          <span w-6 h-6 rounded-3 bg-black dark:bg-white />
        </div>
      </div>
      <div w-50 h-50 b-1 rounded-5 flex-col justify-between p-10 m-20>
        <div flex w-full justify-between>
          <span w-6 h-6 rounded-3 bg-black dark:bg-white />
          <span w-6 h-6 rounded-3 bg-black dark:bg-white />
        </div>
        <div flex w-full justify-between>
          <span w-6 h-6 rounded-3 bg-black dark:bg-white />
          <span w-6 h-6 rounded-3 bg-black dark:bg-white />
        </div>
        <div flex w-full justify-between>
          <span w-6 h-6 rounded-3 bg-black dark:bg-white />
          <span w-6 h-6 rounded-3 bg-black dark:bg-white />
        </div>
      </div>
    </section>

    <p mt-20 text-14 color-gray-400>Flex骰子</p>
  </main>
</template>