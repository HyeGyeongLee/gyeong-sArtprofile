<template>
    <div class="bg-white py-0 sm:py-0">
      <div class="mx-auto px-6 lg:px-8">
        <!-- <div class="mx-auto max-w-2xl lg:mx-0">
          <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl"></h2>
          <p class="mt-6 text-lg leading-8 text-gray-600">We’re a dynamic group of individuals who are passionate about what we do and dedicated to delivering the best results for our clients.</p>
        </div> -->
        <ul role="list" class="mx-auto mt-0 grid max-w-2xl grid-cols-2 gap-x-1 gap-y-1 sm:grid-cols-2 lg:mx-0 lg:max-w-none lg:grid-cols-4">
          <li v-for="person in people" :key="person.name">
            <img class="w-[100%] h-full" :src="person.imageUrl" alt="" />
          </li>
        </ul>
      </div>
    </div>
  </template>
  
  <script setup>
  const people = [
  {
      imageUrl:
        '/work/work9.jpeg',
    },
  {
      imageUrl:
        '/work/work8.jpeg',
    },
  {
      imageUrl:
        '/work/work7.jpeg',
    },
  {
      imageUrl:
        '/work/work6.jpeg',
    },
  {
      imageUrl:
        '/work/work5.jpeg',
    },
  {
      imageUrl:
        '/work/work4.jpeg',
    },
  {
      imageUrl:
        '/work/work3.jpeg',
    },
  {
      imageUrl:
        '/work/work2.jpeg',
    },
  {
      imageUrl:
        '/work/work1.jpeg',
    },
    {
      imageUrl:
        '/main/main1.jpeg',
    },
    {
      imageUrl:
        '/main/main2.jpeg',
    },
    {
      imageUrl:
        '/main/main3.jpeg',
    },
    {
      imageUrl:
        '/main/main4.jpeg',
    },
    {
      imageUrl:
        '/main/main5.jpeg',
    },
    {
      imageUrl:
        '/main/main6.jpeg',
    },
    {
      imageUrl:
        '/main/main7.jpeg',
    },
    {
      imageUrl:
        '/main/main8.jpeg',
    },
    // More people...
  ]
  </script>