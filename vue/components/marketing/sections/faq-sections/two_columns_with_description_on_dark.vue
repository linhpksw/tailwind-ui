<!-- This example requires Tailwind CSS v2.0+ -->
<template>
  <div class="bg-gray-900">
    <div class="mx-auto max-w-7xl py-16 px-4 sm:py-24 sm:px-6 lg:px-8">
      <div class="lg:mx-auto lg:max-w-2xl lg:text-center">
        <h2 class="text-3xl font-bold tracking-tight text-white sm:text-4xl">Frequently asked questions</h2>
        <p class="mt-4 text-gray-400">Ac euismod vel sit maecenas id pellentesque eu sed consectetur. Malesuada adipiscing sagittis vel nulla nec. Urna, sed a lectus elementum blandit et.</p>
      </div>
      <div class="mt-20">
        <dl class="space-y-10 lg:grid lg:grid-cols-2 lg:gap-x-8 lg:gap-y-10 lg:space-y-0">
          <div v-for="faq in faqs" :key="faq.id">
            <dt class="font-semibold text-white">{{ faq.question }}</dt>
            <dd class="mt-3 text-gray-400">{{ faq.answer }}</dd>
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