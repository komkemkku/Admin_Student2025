<template>
  <div class="flex min-h-screen">
    <!-- Left Side -->
    <div class="w-2/3 bg-gray-300"></div>

    <!-- Right Side (Login Form) -->
    <div class="w-1/3 bg-white flex flex-col items-center p-10">
      <!-- Logo -->
      <div class="font-serif text-center mt-10">
        <h1 class="text-4xl font-bold text-black">KhonKaen</h1>
        <h2 class="text-lg text-black">University</h2>
      </div>

      <!-- Login Form -->
      <div class="flex flex-col items-center justify-center w-full mt-10">
        <h1 class="font-serif text-2xl font-bold mt-6">Login</h1>

        <div class="w-full max-w-sm mt-10">
          <label class="block text-sm font-semibold">Username :</label>
          <input
            type="text"
            class="w-full p-4 mt-2 bg-gray-200 border border-gray-300 rounded-3xl drop-shadow-lg"
            placeholder="username"
          />

          <label class="block mt-4 text-sm font-semibold">Password :</label>
          <input
            type="password"
            class="w-full p-4 mt-2 bg-gray-200 border border-gray-300 rounded-3xl drop-shadow-lg"
            placeholder="password"
          />

          <!-- Login Button -->
          <div class="flex justify-center mt-6">
            <button
              class="font-serif font-bold text-xl text-white bg-black w-40 h-10 rounded-3xl hover:bg-gray-800 transition mt-20"
            >
              Login
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup></script>

<style></style>
