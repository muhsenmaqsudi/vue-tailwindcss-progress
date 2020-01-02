---
uuid: base
name: Kanban Board
published_at: null
category: Page Layouts
subcategory: Application UI
---

<template>
  <div class="h-screen flex">
    <div
      :class="
        sidebarOpen
          ? 'translate-x-0 animation-ease-out animation-normal'
          : '-translate-x-full animation-ease-in animation-normal'
      "
      class="fixed z-30 inset-y-0 left-0 w-64 px-8 py-4 bg-gray-100 border-r border-r overflow-auto lg:static lg:inset-auto lg:translate-x-0"
    >
      <div class="-mx-3 pl-3 pr-1 flex items-center justify-between">
        <span>
          <img class="h-8 w-8" src="@/assets/logo.png" alt="vuejs logo" />
        </span>
        <button class="text-gray-700 lg:hidden" @click="sidebarOpen = false">
          <svg class="h-6 w-6" viewBox="0 0 24 24" fill="none">
            <path
              stroke="currentColor"
              stroke-width="2"
              stroke-linecap="round"
              d="M6 18L18 6M6 6L18 18"
            ></path>
          </svg>
        </button>
      </div>

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

    <div class="flex-1 min-w-0 bg-white overflow-auto">
      <div class="flex-shrink-0 border-b-2 border-gray-200">
        <header class="px-6">
          <div class="flex justify-between items-center py-3 border-b border-gray-200">
            <div class="flex flex-1">
              <button class="text-gray-600 lg:hidden" @click="sidebarOpen = true">
                <svg class="h-6 w-6" viewBox="0 0 24 24" fill="none">
                  <path
                    stroke="currentColor"
                    stroke-width="2"
                    stroke-linecap="round"
                    d="M4 6h16M4 12h16M4 18h7"
                  />
                </svg>
              </button>
              <div class="ml-3 relative w-64 lg:ml-0">
                <span class="absolute inset-y-0 left-0 pl-3 flex items-center">
                  <svg class="h-6 w-6 text-gray-600" viewBox="0 0 24 24" fill="none">
                    <path
                      stroke="currentColor"
                      stroke-width="2"
                      stroke-linecap="round"
                      d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"
                    />
                  </svg>
                </span>

                <input
                  class="block w-full rounder-md border border-gray-400 pl-10 pr-4 py-2 text-sm text-gray-900 placeholder-gray-600"
                  placeholder="Search"
                />
              </div>
            </div>
            <div class="flex items-center">
              <button>
                <svg class="h-6 w-6 text-gray-600" viewBox="0 0 24 24" fill="none">
                  <path
                    stroke="currentColor"
                    stroke-width="2"
                    stroke-linecap="round"
                    d="M15.137 3.945c-.644-.374-1.042-1.07-1.041-1.82v-.003c.001-1.172-.938-2.122-2.096-2.122s-2.097.95-2.097 2.122v.003c.001.751-.396 1.446-1.041 1.82-4.667 2.712-1.985 11.715-6.862 13.306v1.749h20v-1.749c-4.877-1.591-2.195-10.594-6.863-13.306zm-3.137-2.945c.552 0 1 .449 1 1 0 .552-.448 1-1 1s-1-.448-1-1c0-.551.448-1 1-1zm3 20c0 1.598-1.392 3-2.971 3s-3.029-1.402-3.029-3h6z"
                  />
                </svg>
              </button>
              <button class="ml-6">
                <img
                  class="h-10 w-10 rounded-full object-cover"
                  src="https://images.unsplash.com/photo-1487412720507-e7ab37603c6f?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                  alt="Your profile image"
                />
              </button>
            </div>
          </div>
          <div class="ml-6 flex items-center justify-between py-2">
            <div class="flex items-center">
              <h2 class="text-xl font-semibold text-gray-900 leading-tight">
                All Issues
              </h2>
              <div class="ml-6 flex items-center">
                <span class="rounded-full border-2 border-white">
                  <img
                    class="-ml-2 h-6 w-6 rounded-full object-cover "
                    src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                    alt=""
                  />
                </span>
                <span class="rounded-full border-2 border-white">
                  <img
                    class="-ml-2 h-6 w-6 rounded-full object-cover "
                    src="https://images.unsplash.com/photo-1511367461989-f85a21fda167?ixlib=rb-1.2.1&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                    alt=""
                  />
                </span>
                <span class="rounded-full border-2 border-white">
                  <img
                    class="-ml-2 h-6 w-6 rounded-full object-cover "
                    src="https://images.unsplash.com/photo-1455274111113-575d080ce8cd?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                    alt=""
                  />
                </span>
                <span class="rounded-full border-2 border-white">
                  <img
                    class="-ml-2 h-6 w-6 rounded-full object-cover "
                    src="https://images.unsplash.com/photo-1532074205216-d0e1f4b87368?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                    alt=""
                  />
                </span>
              </div>
            </div>
            <div class="flex">
              <span class="inline-flex p-1 border bg-gray-200 rounded-md">
                <button class="-m-px px-2 py-1 rounded">
                  <svg class="h-6 w-6 text-gray-600" viewBox="0 0 24 24" fill="none">
                    <path
                      stroke="currentColor"
                      stroke-width="2"
                      stroke-linecap="round"
                      d="M4 6h16M4 10h16M4 14h16M4 18h16"
                    />
                  </svg>
                </button>
                <button class="-m-px px-2 py-1 bg-white rounded shadow">
                  <svg class="h-6 w-6 text-gray-600" viewBox="0 0 24 24" fill="none">
                    <path
                      stroke="currentColor"
                      stroke-width="2"
                      stroke-linecap="round"
                      d="M9 17V7m0 10a2 2 0 01-2 2H5a2 2 0 01-2-2V7a2 2 0 01-2"
                    />
                  </svg>
                </button>
              </span>
              <button
                class="ml-5 flex items-center pl-2 pr-4 py-2 text-sm font-medium text-white bg-gray-800 rounded hover:bg-gray-700"
              >
                <svg class="h-5 w-5 text-gray-500" viewBox="0 0 24 24" fill="none">
                  <path
                    stroke="currentColor"
                    stroke-width="2"
                    stroke-linecap="round"
                    d="M12 7v10m5-5H7"
                  />
                </svg>
                <span class="ml-1">New Issue</span>
              </button>
            </div>
          </div>
        </header>
      </div>

      <div class="flex-1 h-full">
        <main class="p-3 h-full inline-flex">
          <!-- first column -->
          <div class="flex-shrink-0 flex flex-col py-3 w-64 bg-gray-100 rounded">
            <h3 class="flex-shrink-0 px-3 text-sm font-medium text-gray-700">
              Backlog
            </h3>
            <div class="flex-1 min-h-0 overflow-y-auto">
              <ul class="pt-1 pb-3 px-3">
                <li>
                  <a href="#" class="block p-5 bg-white rounded shadow">
                    <div class="flex justify-between">
                      <p class="text-sm font-medium leading-snug text-gray-900">
                        Add discount code to checkout page
                      </p>
                      <span>
                        <img
                          class="rounded-full h-6 w-6"
                          src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                          alt=""
                        />
                      </span>
                    </div>
                    <div class="flex justify-between items-baseline">
                      <div class="text-sm text-gray-600">
                        <time datetime="2020-01-01">Jan 1</time>
                      </div>
                      <div class="mt-2">
                        <span
                          class="px-2 py-1 leading-tight inline-flex items-center bg-teal-100 rounded"
                        >
                          <svg
                            class="h-2 w-2 text-teal-500"
                            viewBox="0 0 8 8"
                            fill="currentColor"
                          >
                            <circle cx="4" cy="4" r="3" />
                          </svg>
                          <span class="ml-2 text-sm text-teal-900">Feature Request</span>
                        </span>
                      </div>
                    </div>
                  </a>
                </li>
                <li class="mt-3">
                  <a href="#" class="block p-5 bg-white rounded shadow">
                    <div class="flex justify-between">
                      <p class="text-sm font-medium leading-snug text-gray-900">
                        Add discount code to checkout page
                      </p>
                      <span>
                        <img
                          class="rounded-full h-6 w-6"
                          src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                          alt=""
                        />
                      </span>
                    </div>
                    <div class="flex justify-between items-baseline">
                      <div class="text-sm text-gray-600">
                        <time datetime="2020-01-01">Jan 1</time>
                      </div>
                      <div class="mt-2">
                        <span
                          class="px-2 py-1 leading-tight inline-flex items-center bg-teal-100 rounded"
                        >
                          <svg
                            class="h-2 w-2 text-teal-500"
                            viewBox="0 0 8 8"
                            fill="currentColor"
                          >
                            <circle cx="4" cy="4" r="3" />
                          </svg>
                          <span class="ml-2 text-sm text-teal-900">Feature Request</span>
                        </span>
                      </div>
                    </div>
                  </a>
                </li>
                <li class="mt-3">
                  <a href="#" class="block p-5 bg-white rounded shadow">
                    <div class="flex justify-between">
                      <p class="text-sm font-medium leading-snug text-gray-900">
                        Add discount code to checkout page
                      </p>
                      <span>
                        <img
                          class="rounded-full h-6 w-6"
                          src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                          alt=""
                        />
                      </span>
                    </div>
                    <div class="flex justify-between items-baseline">
                      <div class="text-sm text-gray-600">
                        <time datetime="2020-01-01">Jan 1</time>
                      </div>
                      <div class="mt-2">
                        <span
                          class="px-2 py-1 leading-tight inline-flex items-center bg-teal-100 rounded"
                        >
                          <svg
                            class="h-2 w-2 text-teal-500"
                            viewBox="0 0 8 8"
                            fill="currentColor"
                          >
                            <circle cx="4" cy="4" r="3" />
                          </svg>
                          <span class="ml-2 text-sm text-teal-900">Feature Request</span>
                        </span>
                      </div>
                    </div>
                  </a>
                </li>
                <li class="mt-3">
                  <a href="#" class="block p-5 bg-white rounded shadow">
                    <div class="flex justify-between">
                      <p class="text-sm font-medium leading-snug text-gray-900">
                        Add discount code to checkout page
                      </p>
                      <span>
                        <img
                          class="rounded-full h-6 w-6"
                          src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                          alt=""
                        />
                      </span>
                    </div>
                    <div class="flex justify-between items-baseline">
                      <div class="text-sm text-gray-600">
                        <time datetime="2020-01-01">Jan 1</time>
                      </div>
                      <div class="mt-2">
                        <span
                          class="px-2 py-1 leading-tight inline-flex items-center bg-teal-100 rounded"
                        >
                          <svg
                            class="h-2 w-2 text-teal-500"
                            viewBox="0 0 8 8"
                            fill="currentColor"
                          >
                            <circle cx="4" cy="4" r="3" />
                          </svg>
                          <span class="ml-2 text-sm text-teal-900">Feature Request</span>
                        </span>
                      </div>
                    </div>
                  </a>
                </li>
                <li class="mt-3">
                  <a href="#" class="block p-5 bg-white rounded shadow">
                    <div class="flex justify-between">
                      <p class="text-sm font-medium leading-snug text-gray-900">
                        Add discount code to checkout page
                      </p>
                      <span>
                        <img
                          class="rounded-full h-6 w-6"
                          src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                          alt=""
                        />
                      </span>
                    </div>
                    <div class="flex justify-between items-baseline">
                      <div class="text-sm text-gray-600">
                        <time datetime="2020-01-01">Jan 1</time>
                      </div>
                      <div class="mt-2">
                        <span
                          class="px-2 py-1 leading-tight inline-flex items-center bg-teal-100 rounded"
                        >
                          <svg
                            class="h-2 w-2 text-teal-500"
                            viewBox="0 0 8 8"
                            fill="currentColor"
                          >
                            <circle cx="4" cy="4" r="3" />
                          </svg>
                          <span class="ml-2 text-sm text-teal-900">Feature Request</span>
                        </span>
                      </div>
                    </div>
                  </a>
                </li>
              </ul>
            </div>
          </div>
          <!-- end of first column -->
          <!-- 2nd column -->
          <div class="ml-3 flex-shrink-0 flex flex-col py-3 w-64 bg-gray-100 rounded">
            <h3 class="flex-shrink-0 px-3 text-sm font-medium text-gray-700">
              Ready for Review
            </h3>
            <div class="flex-1 min-h-0 overflow-y-auto">
              <ul class="pt-1 pb-3 px-3">
                <li>
                  <a href="#" class="block p-5 bg-white rounded shadow">
                    <div class="flex justify-between">
                      <p class="text-sm font-medium leading-snug text-gray-900">
                        Add discount code to checkout page
                      </p>
                      <span>
                        <img
                          class="rounded-full h-6 w-6"
                          src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                          alt=""
                        />
                      </span>
                    </div>
                    <div class="flex justify-between items-baseline">
                      <div class="text-sm text-gray-600">
                        <time datetime="2020-01-01">Jan 1</time>
                      </div>
                      <div class="mt-2">
                        <span
                          class="px-2 py-1 leading-tight inline-flex items-center bg-teal-100 rounded"
                        >
                          <svg
                            class="h-2 w-2 text-teal-500"
                            viewBox="0 0 8 8"
                            fill="currentColor"
                          >
                            <circle cx="4" cy="4" r="3" />
                          </svg>
                          <span class="ml-2 text-sm text-teal-900">Feature Request</span>
                        </span>
                      </div>
                    </div>
                  </a>
                </li>
                <li class="mt-3">
                  <a href="#" class="block p-5 bg-white rounded shadow">
                    <div class="flex justify-between">
                      <p class="text-sm font-medium leading-snug text-gray-900">
                        Add discount code to checkout page
                      </p>
                      <span>
                        <img
                          class="rounded-full h-6 w-6"
                          src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                          alt=""
                        />
                      </span>
                    </div>
                    <div class="flex justify-between items-baseline">
                      <div class="text-sm text-gray-600">
                        <time datetime="2020-01-01">Jan 1</time>
                      </div>
                      <div class="mt-2">
                        <span
                          class="px-2 py-1 leading-tight inline-flex items-center bg-teal-100 rounded"
                        >
                          <svg
                            class="h-2 w-2 text-teal-500"
                            viewBox="0 0 8 8"
                            fill="currentColor"
                          >
                            <circle cx="4" cy="4" r="3" />
                          </svg>
                          <span class="ml-2 text-sm text-teal-900">Feature Request</span>
                        </span>
                      </div>
                    </div>
                  </a>
                </li>
                <li class="mt-3">
                  <a href="#" class="block p-5 bg-white rounded shadow">
                    <div class="flex justify-between">
                      <p class="text-sm font-medium leading-snug text-gray-900">
                        Add discount code to checkout page
                      </p>
                      <span>
                        <img
                          class="rounded-full h-6 w-6"
                          src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                          alt=""
                        />
                      </span>
                    </div>
                    <div class="flex justify-between items-baseline">
                      <div class="text-sm text-gray-600">
                        <time datetime="2020-01-01">Jan 1</time>
                      </div>
                      <div class="mt-2">
                        <span
                          class="px-2 py-1 leading-tight inline-flex items-center bg-teal-100 rounded"
                        >
                          <svg
                            class="h-2 w-2 text-teal-500"
                            viewBox="0 0 8 8"
                            fill="currentColor"
                          >
                            <circle cx="4" cy="4" r="3" />
                          </svg>
                          <span class="ml-2 text-sm text-teal-900">Feature Request</span>
                        </span>
                      </div>
                    </div>
                  </a>
                </li>
                <li class="mt-3">
                  <a href="#" class="block p-5 bg-white rounded shadow">
                    <div class="flex justify-between">
                      <p class="text-sm font-medium leading-snug text-gray-900">
                        Add discount code to checkout page
                      </p>
                      <span>
                        <img
                          class="rounded-full h-6 w-6"
                          src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                          alt=""
                        />
                      </span>
                    </div>
                    <div class="flex justify-between items-baseline">
                      <div class="text-sm text-gray-600">
                        <time datetime="2020-01-01">Jan 1</time>
                      </div>
                      <div class="mt-2">
                        <span
                          class="px-2 py-1 leading-tight inline-flex items-center bg-teal-100 rounded"
                        >
                          <svg
                            class="h-2 w-2 text-teal-500"
                            viewBox="0 0 8 8"
                            fill="currentColor"
                          >
                            <circle cx="4" cy="4" r="3" />
                          </svg>
                          <span class="ml-2 text-sm text-teal-900">Feature Request</span>
                        </span>
                      </div>
                    </div>
                  </a>
                </li>
                <li class="mt-3">
                  <a href="#" class="block p-5 bg-white rounded shadow">
                    <div class="flex justify-between">
                      <p class="text-sm font-medium leading-snug text-gray-900">
                        Add discount code to checkout page
                      </p>
                      <span>
                        <img
                          class="rounded-full h-6 w-6"
                          src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                          alt=""
                        />
                      </span>
                    </div>
                    <div class="flex justify-between items-baseline">
                      <div class="text-sm text-gray-600">
                        <time datetime="2020-01-01">Jan 1</time>
                      </div>
                      <div class="mt-2">
                        <span
                          class="px-2 py-1 leading-tight inline-flex items-center bg-teal-100 rounded"
                        >
                          <svg
                            class="h-2 w-2 text-teal-500"
                            viewBox="0 0 8 8"
                            fill="currentColor"
                          >
                            <circle cx="4" cy="4" r="3" />
                          </svg>
                          <span class="ml-2 text-sm text-teal-900">Feature Request</span>
                        </span>
                      </div>
                    </div>
                  </a>
                </li>
                <li class="mt-3">
                  <a href="#" class="block p-5 bg-white rounded shadow">
                    <div class="flex justify-between">
                      <p class="text-sm font-medium leading-snug text-gray-900">
                        Add discount code to checkout page
                      </p>
                      <span>
                        <img
                          class="rounded-full h-6 w-6"
                          src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                          alt=""
                        />
                      </span>
                    </div>
                    <div class="flex justify-between items-baseline">
                      <div class="text-sm text-gray-600">
                        <time datetime="2020-01-01">Jan 1</time>
                      </div>
                      <div class="mt-2">
                        <span
                          class="px-2 py-1 leading-tight inline-flex items-center bg-teal-100 rounded"
                        >
                          <svg
                            class="h-2 w-2 text-teal-500"
                            viewBox="0 0 8 8"
                            fill="currentColor"
                          >
                            <circle cx="4" cy="4" r="3" />
                          </svg>
                          <span class="ml-2 text-sm text-teal-900">Feature Request</span>
                        </span>
                      </div>
                    </div>
                  </a>
                </li>
                <li class="mt-3">
                  <a href="#" class="block p-5 bg-white rounded shadow">
                    <div class="flex justify-between">
                      <p class="text-sm font-medium leading-snug text-gray-900">
                        Add discount code to checkout page
                      </p>
                      <span>
                        <img
                          class="rounded-full h-6 w-6"
                          src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                          alt=""
                        />
                      </span>
                    </div>
                    <div class="flex justify-between items-baseline">
                      <div class="text-sm text-gray-600">
                        <time datetime="2020-01-01">Jan 1</time>
                      </div>
                      <div class="mt-2">
                        <span
                          class="px-2 py-1 leading-tight inline-flex items-center bg-teal-100 rounded"
                        >
                          <svg
                            class="h-2 w-2 text-teal-500"
                            viewBox="0 0 8 8"
                            fill="currentColor"
                          >
                            <circle cx="4" cy="4" r="3" />
                          </svg>
                          <span class="ml-2 text-sm text-teal-900">Feature Request</span>
                        </span>
                      </div>
                    </div>
                  </a>
                </li>
                <li class="mt-3">
                  <a href="#" class="block p-5 bg-white rounded shadow">
                    <div class="flex justify-between">
                      <p class="text-sm font-medium leading-snug text-gray-900">
                        Add discount code to checkout page
                      </p>
                      <span>
                        <img
                          class="rounded-full h-6 w-6"
                          src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                          alt=""
                        />
                      </span>
                    </div>
                    <div class="flex justify-between items-baseline">
                      <div class="text-sm text-gray-600">
                        <time datetime="2020-01-01">Jan 1</time>
                      </div>
                      <div class="mt-2">
                        <span
                          class="px-2 py-1 leading-tight inline-flex items-center bg-teal-100 rounded"
                        >
                          <svg
                            class="h-2 w-2 text-teal-500"
                            viewBox="0 0 8 8"
                            fill="currentColor"
                          >
                            <circle cx="4" cy="4" r="3" />
                          </svg>
                          <span class="ml-2 text-sm text-teal-900">Feature Request</span>
                        </span>
                      </div>
                    </div>
                  </a>
                </li>
              </ul>
            </div>
          </div>

          <div class="ml-3 flex-shrink-0 flex flex-col py-3 w-64 bg-gray-100 rounded">
            <h3 class="flex-shrink-0 px-3 text-sm font-medium text-gray-700">
              Doing
            </h3>
            <div class="flex-1 min-h-0 overflow-y-auto">
              <ul class="pt-1 pb-3 px-3">
                <li>
                  <a href="#" class="block p-5 bg-white rounded shadow">
                    <div class="flex justify-between">
                      <p class="text-sm font-medium leading-snug text-gray-900">
                        Add discount code to checkout page
                      </p>
                      <span>
                        <img
                          class="rounded-full h-6 w-6"
                          src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                          alt=""
                        />
                      </span>
                    </div>
                    <div class="flex justify-between items-baseline">
                      <div class="text-sm text-gray-600">
                        <time datetime="2020-01-01">Jan 1</time>
                      </div>
                      <div class="mt-2">
                        <span
                          class="px-2 py-1 leading-tight inline-flex items-center bg-teal-100 rounded"
                        >
                          <svg
                            class="h-2 w-2 text-teal-500"
                            viewBox="0 0 8 8"
                            fill="currentColor"
                          >
                            <circle cx="4" cy="4" r="3" />
                          </svg>
                          <span class="ml-2 text-sm text-teal-900">Feature Request</span>
                        </span>
                      </div>
                    </div>
                  </a>
                </li>
                <li class="mt-3">
                  <a href="#" class="block p-5 bg-white rounded shadow">
                    <div class="flex justify-between">
                      <p class="text-sm font-medium leading-snug text-gray-900">
                        Add discount code to checkout page
                      </p>
                      <span>
                        <img
                          class="rounded-full h-6 w-6"
                          src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                          alt=""
                        />
                      </span>
                    </div>
                    <div class="flex justify-between items-baseline">
                      <div class="text-sm text-gray-600">
                        <time datetime="2020-01-01">Jan 1</time>
                      </div>
                      <div class="mt-2">
                        <span
                          class="px-2 py-1 leading-tight inline-flex items-center bg-teal-100 rounded"
                        >
                          <svg
                            class="h-2 w-2 text-teal-500"
                            viewBox="0 0 8 8"
                            fill="currentColor"
                          >
                            <circle cx="4" cy="4" r="3" />
                          </svg>
                          <span class="ml-2 text-sm text-teal-900">Feature Request</span>
                        </span>
                      </div>
                    </div>
                  </a>
                </li>
              </ul>
            </div>
          </div>
          <div class="ml-3 flex-shrink-0 flex flex-col py-3 w-64 bg-gray-100 rounded">
            <h3 class="flex-shrink-0 px-3 text-sm font-medium text-gray-700">
              Done
            </h3>
            <div class="flex-1 min-h-0 overflow-y-auto">
              <ul class="pt-1 pb-3 px-3">
                <li>
                  <a href="#" class="block p-5 bg-white rounded shadow">
                    <div class="flex justify-between">
                      <p class="text-sm font-medium leading-snug text-gray-900">
                        Add discount code to checkout page
                      </p>
                      <span>
                        <img
                          class="rounded-full h-6 w-6"
                          src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                          alt=""
                        />
                      </span>
                    </div>
                    <div class="flex justify-between items-baseline">
                      <div class="text-sm text-gray-600">
                        <time datetime="2020-01-01">Jan 1</time>
                      </div>
                      <div class="mt-2">
                        <span
                          class="px-2 py-1 leading-tight inline-flex items-center bg-teal-100 rounded"
                        >
                          <svg
                            class="h-2 w-2 text-teal-500"
                            viewBox="0 0 8 8"
                            fill="currentColor"
                          >
                            <circle cx="4" cy="4" r="3" />
                          </svg>
                          <span class="ml-2 text-sm text-teal-900">Feature Request</span>
                        </span>
                      </div>
                    </div>
                  </a>
                </li>
                <li class="mt-3">
                  <a href="#" class="block p-5 bg-white rounded shadow">
                    <div class="flex justify-between">
                      <p class="text-sm font-medium leading-snug text-gray-900">
                        Add discount code to checkout page
                      </p>
                      <span>
                        <img
                          class="rounded-full h-6 w-6"
                          src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                          alt=""
                        />
                      </span>
                    </div>
                    <div class="flex justify-between items-baseline">
                      <div class="text-sm text-gray-600">
                        <time datetime="2020-01-01">Jan 1</time>
                      </div>
                      <div class="mt-2">
                        <span
                          class="px-2 py-1 leading-tight inline-flex items-center bg-teal-100 rounded"
                        >
                          <svg
                            class="h-2 w-2 text-teal-500"
                            viewBox="0 0 8 8"
                            fill="currentColor"
                          >
                            <circle cx="4" cy="4" r="3" />
                          </svg>
                          <span class="ml-2 text-sm text-teal-900">Feature Request</span>
                        </span>
                      </div>
                    </div>
                  </a>
                </li>
                <li class="mt-3">
                  <a href="#" class="block p-5 bg-white rounded shadow">
                    <div class="flex justify-between">
                      <p class="text-sm font-medium leading-snug text-gray-900">
                        Add discount code to checkout page
                      </p>
                      <span>
                        <img
                          class="rounded-full h-6 w-6"
                          src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                          alt=""
                        />
                      </span>
                    </div>
                    <div class="flex justify-between items-baseline">
                      <div class="text-sm text-gray-600">
                        <time datetime="2020-01-01">Jan 1</time>
                      </div>
                      <div class="mt-2">
                        <span
                          class="px-2 py-1 leading-tight inline-flex items-center bg-teal-100 rounded"
                        >
                          <svg
                            class="h-2 w-2 text-teal-500"
                            viewBox="0 0 8 8"
                            fill="currentColor"
                          >
                            <circle cx="4" cy="4" r="3" />
                          </svg>
                          <span class="ml-2 text-sm text-teal-900">Feature Request</span>
                        </span>
                      </div>
                    </div>
                  </a>
                </li>

                <li class="mt-3">
                  <a href="#" class="block p-5 bg-white rounded shadow">
                    <div class="flex justify-between">
                      <p class="text-sm font-medium leading-snug text-gray-900">
                        Add discount code to checkout page
                      </p>
                      <span>
                        <img
                          class="rounded-full h-6 w-6"
                          src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2.25&w=144&h=144&q=80"
                          alt=""
                        />
                      </span>
                    </div>
                    <div class="flex justify-between items-baseline">
                      <div class="text-sm text-gray-600">
                        <time datetime="2020-01-01">Jan 1</time>
                      </div>
                      <div class="mt-2">
                        <span
                          class="px-2 py-1 leading-tight inline-flex items-center bg-teal-100 rounded"
                        >
                          <svg
                            class="h-2 w-2 text-teal-500"
                            viewBox="0 0 8 8"
                            fill="currentColor"
                          >
                            <circle cx="4" cy="4" r="3" />
                          </svg>
                          <span class="ml-2 text-sm text-teal-900">Feature Request</span>
                        </span>
                      </div>
                    </div>
                  </a>
                </li>
              </ul>
            </div>
          </div>
        </main>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'App',
  data() {
    return {
      sidebarOpen: false,
    };
  },
};
</script>
