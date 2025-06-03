<script setup>
defineProps({
  visible: Boolean,
  image: String,
});
defineEmits(["close"]);
</script>
<template>
  <!-- Modal -->
  <div
    v-if="visible"
    class="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center z-50"
  >
    <div class="bg-white p-4 rounded-lg max-w-lg w-full relative">
      <button
        @click="$emit('close')"
        class="absolute top-2 right-2 text-gray-500 hover:text-black"
      >
        &times;
      </button>
      <img :src="image" alt="Modal Image" class="w-full h-auto mt-3" />
    </div>
  </div>
</template>
<style scoped>
.modal-scroll {
  -webkit-overflow-scrolling: touch;
}
</style>
