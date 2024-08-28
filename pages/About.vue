<template>
    <div class="bg-white py-6 md:py-32 md:px-0 px-6 mb-12">
      <div class="mx-auto grid max-w-7xl">
        <div class="max-w-4xl mb-12">
          <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">감정의 색채</h2>
          <p class="mt-6 text-lg font-bold">전시</p>
          <p class="mt-3 text-lg leading-8 text-gray-600 break-keep text-justify">성수 뎁센트2 - 2024</p>
        </div>
        <ul role="list" class="-mt-12 space-y-12 divide-y divide-gray-200 xl:col-span-3">
          <li v-for="person in people" :key="person.name" class="flex flex-col gap-10 pt-12 sm:flex-row">
            <img class="w-[30%] flex-none rounded-2xl object-cover" :src="person.imageUrl" alt="" />
            <div class="max-w-3xl flex-auto relative">
              <h3 class="text-lg font-semibold leading-8 tracking-tight text-gray-900">{{ person.name }}</h3>
              <p class="text-base leading-7 text-gray-600">{{ person.role }}</p>
              <p class="mt-6 sm:text-base sm:leading-9 text-sm leading-6  text-gray-600 break-keep text-justify">{{ person.bio }}</p>
              <ul role="list" class="mt-6 flex gap-x-6 absolute -bottom-6 sm:bottom-0">
                <li>
                    <p class="text-gray-600 text-base">wingedant1@naver.com</p>
                </li>
                <li>
                  <a :href="person.linkedinUrl" target='_blank' class="text-gray-400 hover:text-gray-500">
                    <span class="sr-only">LinkedIn</span>
                    <svg class="h-5 w-5" aria-hidden="true" fill="currentColor" viewBox="0 0 20 20">
                      <path fill-rule="evenodd" d="M16.338 16.338H13.67V12.16c0-.995-.017-2.277-1.387-2.277-1.39 0-1.601 1.086-1.601 2.207v4.248H8.014v-8.59h2.559v1.174h.037c.356-.675 1.227-1.387 2.526-1.387 2.703 0 3.203 1.778 3.203 4.092v4.711zM5.005 6.575a1.548 1.548 0 11-.003-3.096 1.548 1.548 0 01.003 3.096zm-1.337 9.763H6.34v-8.59H3.667v8.59zM17.668 1H2.328C1.595 1 1 1.581 1 2.298v15.403C1 18.418 1.595 19 2.328 19h15.34c.734 0 1.332-.582 1.332-1.299V2.298C19 1.581 18.402 1 17.668 1z" clip-rule="evenodd" />
                    </svg>
                  </a>
                </li>
              </ul>
            </div>
          </li>
        </ul>
      </div>
    </div>
  </template>
  
  <script setup>
  const people = [
    {
      name: 'HyeGyeong Lee',
      role: 'Frontend Developer',
      imageUrl:
        '/about.jpeg',
      bio: `어린 시절부터 예술의 세계에 빠져든 나는 5살 때 처음으로 붓을 잡았습니다. 그 순간부터 그림은 단순한 취미를 넘어 내 삶의 중요한 부분이 되었습니다. 시간이 흐르면서 나의 열정은 더욱 깊어졌고, 이제는 그림이 내 영혼을 표현하는 언어가 되었습니다.
최근에는 같은 꿈을 꾸는 동료 예술가들과 함께 전시회를 열었습니다. 우리의 작품들이 갤러리 벽면을 장식하는 모습을 보며, 어린 시절의 꿈이 현실이 되었음을 실감했습니다. 이 경험은 나에게 큰 자신감을 주었고, 앞으로도 꾸준히 작품 활동을 이어나갈 결심을 하게 되었습니다.
나의 주요 작품 주제는 인물화입니다. 캔버스 위에 그려지는 얼굴들은 단순한 초상화가 아닙니다. 그것은 내가 일상에서 마주치는 다양한 감정들의 투영입니다. 기쁨, 슬픔, 분노, 사랑 등 복잡한 인간의 감정들을 생생한 색채와 섬세한 붓터치로 표현합니다.
나의 작품 제작 과정은 마치 일기를 쓰는 것과 같습니다. 하루하루 겪는 감정의 파도를 색으로 옮기고, 그 색들이 모여 하나의 얼굴을 만들어냅니다. 때로는 밝고 경쾌한 색조로 희망과 기쁨을 노래하기도 하고, 또 다른 날엔 어두운 색채로 내면의 고뇌를 표현하기도 합니다.
이렇게 만들어진 각각의 작품들은 나의 감정 여정을 기록한 지도와도 같습니다. 관람객들은 내 그림을 통해 자신의 감정과 경험을 돌아보고, 때로는 위로받기도 합니다. 이것이 바로 내가 추구하는 예술의 힘이자 목적입니다.
앞으로도 나는 붓과 물감으로 계속해서 나의 이야기를 써내려갈 것입니다. 그림은 나의 과거이자 현재, 그리고 미래입니다. 각 작품이 완성될 때마다, 나는 조금씩 성장하고 있음을 느낍니다. 이 여정이 언제까지 이어질지 모르지만, 나는 내 감정의 색채를 세상과 나누는 일을 멈추지 않을 것입니다.`,
      linkedinUrl: 'https://www.instagram.com/bamzrara_/',
    },
    // More people...
  ]
  </script>