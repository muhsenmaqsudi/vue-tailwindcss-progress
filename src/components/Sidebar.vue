<template>
  <div class="w-64 px-8 py-4 bg-gray-100 border-r border-r overflow-auto">
    <img class="h-8 w-8" src="@/assets/logo.png" alt="vuejs logo" />
    <nav class="mt-8">
      <h3 class="text-xs font-semibold text-gray-600 uppercase tracking-wide">
        Issues
      </h3>
      <div class="mt-2 -mx-3">
        <a
          href="#"
          class="flex justify-between items-center px-3 py-2 bg-gray-200 rounded-lg"
        >
          <p class="text-sm font-medium text-gray-900">All</p>
          <span class="text-xs font-semibold text-gray-700">36</span>
        </a>
        <a href="#" class="flex justify-between items-center px-3 py-2 rounded-lg">
          <p class="text-sm font-medium text-gray-700">Assigned to me</p>
          <span class="text-xs font-semibold text-gray-700">2</span>
        </a>
        <a href="#" class="flex justify-between items-center px-3 py-2 rounded-lg">
          <p class="text-sm font-medium text-gray-700">Created by me</p>
          <span class="text-xs font-semibold text-gray-700">1</span>
        </a>
        <a href="#" class="flex justify-between items-center px-3 py-2 rounded-lg">
          <p class="text-sm font-medium text-gray-700">Archived</p>
          <span class="text-xs font-semibold text-gray-700"></span>
        </a>
      </div>

      <h3 class="mt-8 text-xs font-semibold text-gray-600 uppercase tracking-wide">
        Tags
      </h3>
      <div class="mt-2 -mx-3">
        <a href="#" class="flex justify-between items-center px-3 py-2 rounded-lg">
          <p class="text-sm font-medium text-gray-700">Bug</p>
        </a>
        <a href="#" class="flex justify-between items-center px-3 py-2 rounded-lg">
          <p class="text-sm font-medium text-gray-700">Feature Request</p>
        </a>
        <a href="#" class="flex justify-between items-center px-3 py-2 rounded-lg">
          <p class="text-sm font-medium text-gray-700">Marketing</p>
        </a>
        <a href="#" class="flex justify-between items-center px-3 py-2 rounded-lg">
          <p class="text-sm font-medium text-gray-700">v2.0</p>
        </a>
        <a href="#" class="flex justify-between items-center px-3 py-2 rounded-lg">
          <p class="text-sm font-medium text-gray-700">Enhancement</p>
        </a>
        <a href="#" class="flex justify-between items-center px-3 py-2 rounded-lg">
          <p class="text-sm font-medium text-gray-700">Design</p>
        </a>
      </div>
      <button class="mt-2 -ml-2 flex items-center text-sm font-medium text-gray-600">
        <svg class="h-5 w-5 text-gray-500" viewBox="0 0 24 24" fill="none">
          <path
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            d="M12 7v10m5-5H7"
          />
        </svg>
        <span class="ml-1">New Project</span>
      </button>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'Sidebar',
};
</script>
