<!-- This example requires Tailwind CSS v2.0+ -->
<template>
  <div class="bg-white py-12">
    <div class="mx-auto max-w-xl px-4 sm:px-6 lg:max-w-7xl lg:px-8">
      <h2 class="sr-only">A better way to send money.</h2>
      <dl class="space-y-10 lg:grid lg:grid-cols-3 lg:gap-8 lg:space-y-0">
        <div v-for="feature in features" :key="feature.name">
          <dt>
            <div class="flex h-12 w-12 items-center justify-center rounded-md bg-indigo-500 text-white">
              <component :is="feature.icon" class="h-6 w-6" aria-hidden="true" />
            </div>
            <p class="mt-5 text-lg font-medium leading-6 text-gray-900">{{ feature.name }}</p>
          </dt>
          <dd class="mt-2 text-base text-gray-500">{{ feature.description }}</dd>
        </div>
      </dl>
    </div>
  </div>
</template>

<script setup>
import { BoltIcon, GlobeAltIcon, ScaleIcon } from '@heroicons/vue/24/outline'

const features = [
  {
    name: 'Competitive exchange rates',
    description:
      'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Maiores impedit perferendis suscipit eaque, iste dolor cupiditate blanditiis ratione.',
    icon: GlobeAltIcon,
  },
  {
    name: 'No hidden fees',
    description:
      'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Maiores impedit perferendis suscipit eaque, iste dolor cupiditate blanditiis ratione.',
    icon: ScaleIcon,
  },
  {
    name: 'Transfers are instant',
    description:
      'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Maiores impedit perferendis suscipit eaque, iste dolor cupiditate blanditiis ratione.',
    icon: BoltIcon,
  },
]
</script>