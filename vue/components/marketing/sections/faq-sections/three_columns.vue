<!-- This example requires Tailwind CSS v2.0+ -->
<template>
  <div class="bg-white">
    <div class="mx-auto max-w-7xl py-16 px-4 sm:py-24 sm:px-6 lg:px-8">
      <h2 class="text-center text-3xl font-bold tracking-tight text-gray-900">Frequently asked questions</h2>
      <div class="mt-12">
        <dl class="space-y-10 md:grid md:grid-cols-2 md:gap-x-8 md:gap-y-12 md:space-y-0 lg:grid-cols-3">
          <div v-for="faq in faqs" :key="faq.id">
            <dt class="text-lg font-medium leading-6 text-gray-900">{{ faq.question }}</dt>
            <dd class="mt-2 text-base text-gray-500">{{ faq.answer }}</dd>
          </div>
        </dl>
      </div>
    </div>
  </div>
</template>

<script setup>
const faqs = [
  {
    id: 1,
    question: "What's the best thing about Switzerland?",
    answer:
      "I don't know, but the flag is a big plus. Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas cupiditate laboriosam fugiat.",
  },
  // More questions...
]
</script>