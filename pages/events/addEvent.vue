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

    <!-- Main Content -->
    <div class="flex-1 p-10">
      <!-- Header -->
      <div class="flex items-center justify-between">
        <button class="text-3xl font-bold">&larr;</button>
        <h1 class="text-3xl font-bold text-black text-center flex-grow">
          Add Activities
        </h1>
        <div class="flex items-center space-x-2">
          <p class="text-sm font-semibold">Status</p>
          <input type="checkbox" class="toggle" />
        </div>
      </div>

      <!-- Form -->
      <div class="mt-4">
        <label class="text-sm font-semibold">E-ticket</label>
        <div class="relative p-26 bg-gray-300 rounded-lg">
          <button class="absolute top-2 right-2">
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

        <div class="mt-2">
          <div>
            <div>
              <p class="text-sm font-semibold">Activity Name :</p>
              <input
                type="text"
                class="w-[530px] p-3 mt-1 bg-gray-200 border border-gray-300 rounded-md"
              />
            </div>
          </div>
        </div>

        <div class="grid grid-cols-2 gap-4 mt-2">
          <div class="flex justify-between">
            <div>
              <p class="text-sm font-semibold">Location :</p>
              <input
                type="text"
                class="w-[530px] p-3 mt-1 bg-gray-200 border border-gray-300 rounded-md"
              />
            </div>
            <div class="mx-6">
              <p class="text-sm font-semibold">Dress :</p>
              <input
                type="text"
                class="w-[400px] p-3 mt-1 bg-gray-200 border border-gray-300 rounded-md"
              />
            </div>
          </div>
        </div>

        <div class="mt-2">
          <p class="text-sm font-semibold">Description :</p>
          <textarea
            class="w-full p-3 mt-1 bg-gray-200 border border-gray-300 rounded-md"
          ></textarea>
        </div>

        <div class="mt-2">
          <div class="flex">
            <div>
              <p class="text-sm font-semibold">Start Time :</p>
              <input
                type="time"
                class="w-full p-3 mt-1 bg-gray-200 border border-gray-300 rounded-md"
              />
            </div>
            <div class="mx-15">
              <p class="text-sm font-semibold">End Time :</p>
              <input
                type="time"
                class="w-full p-3 mt-1 bg-gray-200 border border-gray-300 rounded-md"
              />
            </div>
          </div>
        </div>

        <div class="grid grid-cols-2 gap-4 mt-2">
          <div class="flex">
            <div>
              <p class="text-sm font-semibold">Start Date :</p>
              <input
                type="date"
                class="w-full p-3 mt-1 bg-gray-200 border border-gray-300 rounded-md"
              />
            </div>
            <div class="mx-7">
              <p class="text-sm font-semibold">End Date :</p>
              <input
                type="date"
                class="w-full p-3 mt-1 bg-gray-200 border border-gray-300 rounded-md"
              />
            </div>
          </div>
        </div>

        <div class="flex justify-center mt-6">
          <button
            class="w-[150px] bg-black text-white py-3 rounded-3xl hover:bg-gray-800"
          >
            Save
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup></script>

<style>
.toggle {
  appearance: none;
  width: 40px;
  height: 20px;
  background: #ccc;
  border-radius: 10px;
  position: relative;
  transition: background 0.3s;
}
.toggle:checked {
  background: black;
}
.toggle:before {
  content: "";
  position: absolute;
  top: 2px;
  left: 2px;
  width: 16px;
  height: 16px;
  background: white;
  border-radius: 50%;
  transition: 0.3s;
}
.toggle:checked:before {
  left: 22px;
}
</style>
