---
uuid: base
name: Kanban Board
published_at: null
category: Page Layouts
subcategory: Application UI
---

<template>
  <div class="h-screen flex">
    <sidebar></sidebar>
    <div class="flex-1 min-w-0 bg-white overflow-auto">
      <top-header></top-header>
      <div class="flex-1 h-full">
        <main class="p-3 h-full w-full inline-flex">
          <!-- first column -->
          <div class="flex-shrink-0 flex flex-col py-3 w-3/12 bg-gray-100 rounded">
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
          <div class="ml-3 flex-shrink-0 flex flex-col py-3 w-3/12 bg-gray-100 rounded">
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

          <div class="ml-3 flex-shrink-0 flex flex-col py-3 w-3/12 bg-gray-100 rounded">
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
          <div class="ml-3 flex-shrink-0 flex flex-col py-3 w-3/12 bg-gray-100 rounded">
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
import Sidebar from '@/components/Sidebar';
import Header from '@/components/Header';
export default {
  name: 'App',
  components: { sidebar: Sidebar, 'top-header': Header },
};
</script>
