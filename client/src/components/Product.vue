<template>
  <div>
    <router-link
      :to="`/product/${product.id}`"
      class="block relative h-48 rounded overflow-hidden"
    >
      <img
        :src="product.thumbnail"
        class="object-cover object-center w-full h-full block"
      />
    </router-link>
    <div class="mt-3">
      <p class="mb-2 text-blue-600 text-xl font-bold">$ {{ product.price }}</p>
      <h2 class="text-gray-900 text-lg font-medium">{{ product.title }}</h2>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Product',
  props: ['product'],
};
</script>
