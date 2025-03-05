<template>
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

    <!-- Content Section -->
    <div class="flex-1 p-10">
      <h1 class="text-center text-3xl font-bold">Banner & Publish</h1>

      <!-- Banner Section -->
      <div class="mt-10">
        <h2 class="text-lg font-semibold">Banner</h2>
        <div class="relative mt-2 p-26 bg-gray-300 rounded-lg">
          <!-- Edit Icon (SVG) -->
          <button class="absolute top-2 right-2 text-gray-600 hover:text-black">
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
                d="m16.862 4.487 1.687-1.688a1.875 1.875 0 1 1 2.652 2.652L10.582 16.07a4.5 4.5 0 0 1-1.897 1.13L6 18l.8-2.685a4.5 4.5 0 0 1 1.13-1.897l8.932-8.931Z"
              />
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M18 14v4.75A2.25 2.25 0 0 1 15.75 21H5.25A2.25 2.25 0 0 1 3 18.75V8.25A2.25 2.25 0 0 1 5.25 6H10"
              />
            </svg>
          </button>
        </div>
        <div class="flex justify-center mt-4">
          <button
            class="w-[100px] bg-black text-white py-3 rounded-3xl hover:bg-gray-800"
          >
            Save
          </button>
        </div>
      </div>

      <!-- Publish Section -->
      <div class="mt-10">
        <h2 class="text-lg font-semibold">Publish</h2>
        <div class="relative mt-2 p-26 bg-gray-300 rounded-lg">
          <!-- Edit Icon (SVG) -->
          <button class="absolute top-2 right-2 text-gray-600 hover:text-black">
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
                d="m16.862 4.487 1.687-1.688a1.875 1.875 0 1 1 2.652 2.652L10.582 16.07a4.5 4.5 0 0 1-1.897 1.13L6 18l.8-2.685a4.5 4.5 0 0 1 1.13-1.897l8.932-8.931Z"
              />
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M18 14v4.75A2.25 2.25 0 0 1 15.75 21H5.25A2.25 2.25 0 0 1 3 18.75V8.25A2.25 2.25 0 0 1 5.25 6H10"
              />
            </svg>
          </button>
        </div>
        <div class="flex justify-center mt-4">
          <button
            class="w-[100px] bg-black text-white py-3 rounded-3xl hover:bg-gray-800"
          >
            Save
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup></script>

<style></style>
