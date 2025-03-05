<template>
  <div>
    <div class="flex min-h-screen bg-gray-100">
      <!-- Sidebar -->
      <div
        class="w-full md:w-1/4 bg-gray-300 p-6 flex flex-col justify-between min-h-screen"
      >
        <!-- Top Section -->
        <div>
          <div class="font-serif flex flex-col items-center">
            <h1 class="text-3xl font-bold text-black">KhonKaen</h1>
            <h2 class="text-lg text-black">University</h2>
          </div>
          <nav class="mt-10 flex flex-col items-center gap-4">
            <button
              class="w-[150px] bg-black text-white py-3 rounded-3xl hover:bg-gray-800"
            >
              Home
            </button>
            <button
              class="w-[150px] bg-black text-white py-3 rounded-3xl hover:bg-gray-800"
            >
              Banner & Publish
            </button>
            <button
              class="w-[150px] bg-black text-white py-3 rounded-3xl hover:bg-gray-800"
            >
              Activities
            </button>
            <button
              class="w-[150px] bg-black text-white py-3 rounded-3xl hover:bg-gray-800"
            >
              Staff
            </button>
            <button
              class="w-[150px] bg-black text-white py-3 rounded-3xl hover:bg-gray-800"
            >
              Report
            </button>
          </nav>
        </div>

        <!-- Logout Button -->
        <button
          class="w-[100px] bg-black text-white py-3 rounded-3xl hover:bg-gray-800 mt-auto mx-auto"
        >
          Log out
        </button>
      </div>
      <!-- Main Content -->
      <div class="flex-1 p-10">
        <div class="flex justify-center">
          <h1 class="text-4xl font-bold text-black">Staff</h1>
        </div>
        <div class="flex justify-end">
          <button
            @click="openPopup"
            class="bg-black text-white py-2 px-4 rounded-3xl hover:bg-gray-800"
          >
            Add
          </button>
        </div>

        <!-- List -->
        <div class="mt-6">
          <div class="flex gap-15 border-b pb-2 font-semibold">
            <p>ID</p>
            <p>Username</p>
          </div>
          <div v-for="(user, index) in users" :key="index">
            <div class="flex justify-between items-center py-2">
              <div class="flex gap-17">
                <p class="font-normal">{{ user.id }}</p>
                <p class="font-normal">{{ user.username }}</p>
              </div>
              <button @click="openPopup" class="text-gray-700 hover:text-black">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke-width="1.5"
                  stroke="currentColor"
                  class="w-6 h-6"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    d="m16.862 4.487 1.687-1.688a1.875 1.875 0 1 1 2.652 2.652L10.582 16.07a4.5 4.5 0 0 1-1.897 1.13L6 18l.8-2.685a4.5 4.5 0 0 1 1.13-1.897l8.932-8.931Zm0 0L19.5 7.125M18 14v4.75A2.25 2.25 0 0 1 15.75 21H5.25A2.25 2.25 0 0 1 3 18.75V8.25A2.25 2.25 0 0 1 5.25 6H10"
                  />
                </svg>
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
    <PopupaddStaff v-if="isPopupOpen" @close="closePopup" />
  </div>
</template>

<script lang="ts" setup>
import { ref } from "vue";

interface User {
  id: number;
  username: string;
}

const users = ref<User[]>([
  { id: 1, username: "komkem" },
  { id: 2, username: "panthita" },
  { id: 3, username: "emoji" },
]);

// State สำหรับเปิด/ปิด Popup
const isPopupOpen = ref(false);

const openPopup = () => {
  isPopupOpen.value = true;
};

const closePopup = () => {
  isPopupOpen.value = false;
};
</script>

<style></style>
