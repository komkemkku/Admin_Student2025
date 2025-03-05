<template>
  <div
    class="fixed inset-0 flex items-center justify-center bg-black bg-opacity-50"
  >
    <div class="bg-white p-6 rounded-lg shadow-lg w-96">
      <h2 class="text-xl font-bold mb-4 text-center">Add Staff</h2>

      <!-- ฟอร์มกรอกข้อมูล -->
      <div>
        <label class="block text-sm font-semibold">Username :</label>
        <input
          type="text"
          class="w-full p-3 mt-1 bg-gray-200 border border-gray-300 rounded-md"
        />

        <label class="block mt-4 text-sm font-semibold">Password :</label>
        <input
          type="password"
          class="w-full p-3 mt-1 bg-gray-200 border border-gray-300 rounded-md"
        />
      </div>

      <!-- ปุ่ม -->
      <div class="flex justify-center gap-4 mt-6">
        <button
          @click="$emit('close')"
          class="bg-gray-600 text-white py-2 px-4 rounded-3xl hover:bg-gray-700"
        >
          Cancel
        </button>
        <button
          class="bg-black text-white py-2 px-4 rounded-3xl hover:bg-gray-800"
        >
          Add
        </button>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
defineEmits(["close"]);
</script>

<style></style>
