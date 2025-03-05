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

      <!-- Dashboard Content -->
      <div class="flex-1 p-10">
        <h1 class="flex justify-center text-4xl font-bold text-black">
          Dashboard
        </h1>

        <!-- Card Section -->
        <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mt-10">
          <div class="p-16 bg-gray-300 rounded-lg"></div>
          <div class="p-16 bg-gray-300 rounded-lg"></div>
          <div class="p-16 bg-gray-300 rounded-lg"></div>
          <div class="p-16 bg-gray-300 rounded-lg"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup></script>

<style></style>
