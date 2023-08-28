<script setup>
import AdminLayout from "@/Layouts/AdminLayout.vue";
import { Head } from "@inertiajs/vue3";
</script>

<template>
    <Head title="Dashboard" />

    <AdminLayout>
        <template #header>
            <h2 class="font-semibold text-xl text-gray-800 leading-tight">
                Dashboard
            </h2>
        </template>

        <div class="py-1">
            <div class="max-w-7xl mx-auto sm:px-6 lg:px-8">
                <!-- <div class="bg-white overflow-hidden shadow-sm sm:rounded-lg">
                    <div class="p-6 text-gray-900">You're logged in!</div>
                </div> -->
                <!-- component -->
                <!-- This is an example component -->
                <!-- component -->
                <div
                    class="min-w-screen bg-gray-100 flex items-center justify-center bg-white-600"
                >
                    <div class="max-w-7xl w-full mx-auto py-6 sm:px-6 lg:px-8">
                        <div
                            class="flex flex-col lg:flex-row w-full lg:space-x-2 space-y-2 lg:space-y-0 mb-2 lg:mb-4"
                        >
                            <div class="w-full lg:w-1/5">
                                <div
                                    class="widget w-full p-4 rounded-lg bg-white border-l-4 border-purple-400"
                                >
                                    <div class="flex items-center">
                                        <div
                                            class="icon w-14 p-3.5 bg-purple-400 text-white rounded-full mr-3"
                                        >
                                            <svg
                                                fill="none"
                                                viewBox="0 0 24 24"
                                                stroke="currentColor"
                                            >
                                                <path
                                                    stroke-linecap="round"
                                                    stroke-linejoin="round"
                                                    stroke-width="2"
                                                    d="M13 7h8m0 0v8m0-8l-8 8-4-4-6 6"
                                                ></path>
                                            </svg>
                                        </div>
                                        <div
                                            class="flex flex-col justify-center"
                                        >
                                            <div class="text-lg">230k</div>
                                            <div class="text-sm text-gray-400">
                                                Sales
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>

                            <div class="w-full lg:w-1/5">
                                <div
                                    class="widget w-full p-4 rounded-lg bg-white border-l-4 border-blue-400"
                                >
                                    <div class="flex items-center">
                                        <div
                                            class="icon w-14 p-3.5 bg-blue-400 text-white rounded-full mr-3"
                                        >
                                            <svg
                                                fill="none"
                                                viewBox="0 0 24 24"
                                                stroke="currentColor"
                                            >
                                                <path
                                                    stroke-linecap="round"
                                                    stroke-linejoin="round"
                                                    stroke-width="2"
                                                    d="M12 4.354a4 4 0 110 5.292M15 21H3v-1a6 6 0 0112 0v1zm0 0h6v-1a6 6 0 00-9-5.197M13 7a4 4 0 11-8 0 4 4 0 018 0z"
                                                />
                                            </svg>
                                        </div>
                                        <div
                                            class="flex flex-col justify-center"
                                        >
                                            <div class="text-lg">3456</div>
                                            <div class="text-sm text-gray-400">
                                                Customers
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>

                            <div class="w-full lg:w-1/5">
                                <div
                                    class="widget w-full p-4 rounded-lg bg-white border-l-4 border-yellow-400"
                                >
                                    <div class="flex items-center">
                                        <div
                                            class="icon w-14 p-3.5 bg-yellow-400 text-white rounded-full mr-3"
                                        >
                                            <svg
                                                fill="none"
                                                viewBox="0 0 24 24"
                                                stroke="currentColor"
                                            >
                                                <path
                                                    stroke-linecap="round"
                                                    stroke-linejoin="round"
                                                    stroke-width="2"
                                                    d="M5 8h14M5 8a2 2 0 110-4h14a2 2 0 110 4M5 8v10a2 2 0 002 2h10a2 2 0 002-2V8m-9 4h4"
                                                />
                                            </svg>
                                        </div>
                                        <div
                                            class="flex flex-col justify-center"
                                        >
                                            <div class="text-lg">3456</div>
                                            <div class="text-sm text-gray-400">
                                                Products
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>

                            <div class="w-full lg:w-1/5">
                                <div
                                    class="widget w-full p-4 rounded-lg bg-white border-l-4 border-red-400"
                                >
                                    <div class="flex items-center">
                                        <div
                                            class="icon w-14 p-3.5 bg-red-400 text-white rounded-full mr-3"
                                        >
                                            <svg
                                                fill="none"
                                                viewBox="0 0 24 24"
                                                stroke="currentColor"
                                            >
                                                <path
                                                    stroke-linecap="round"
                                                    stroke-linejoin="round"
                                                    stroke-width="2"
                                                    d="M3 3h2l.4 2M7 13h10l4-8H5.4M7 13L5.4 5M7 13l-2.293 2.293c-.63.63-.184 1.707.707 1.707H17m0 0a2 2 0 100 4 2 2 0 000-4zm-8 2a2 2 0 11-4 0 2 2 0 014 0z"
                                                />
                                            </svg>
                                        </div>
                                        <div
                                            class="flex flex-col justify-center"
                                        >
                                            <div class="text-lg">12658</div>
                                            <div class="text-sm text-gray-400">
                                                Orders
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>

                            <div class="w-full lg:w-1/5">
                                <div
                                    class="widget w-full p-4 rounded-lg bg-white border-l-4 border-green-400"
                                >
                                    <div class="flex items-center">
                                        <div
                                            class="icon w-14 p-3.5 bg-green-400 text-white rounded-full mr-3"
                                        >
                                            <svg
                                                fill="none"
                                                viewBox="0 0 24 24"
                                                stroke="currentColor"
                                            >
                                                <path
                                                    stroke-linecap="round"
                                                    stroke-linejoin="round"
                                                    stroke-width="2"
                                                    d="M12 8c-1.657 0-3 .895-3 2s1.343 2 3 2 3 .895 3 2-1.343 2-3 2m0-8c1.11 0 2.08.402 2.599 1M12 8V7m0 1v8m0 0v1m0-1c-1.11 0-2.08-.402-2.599-1M21 12a9 9 0 11-18 0 9 9 0 0118 0z"
                                                />
                                            </svg>
                                        </div>
                                        <div
                                            class="flex flex-col justify-center"
                                        >
                                            <div class="text-lg">$948'560</div>
                                            <div class="text-sm text-gray-400">
                                                Revenue
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <!-- Graphs -->
                <div class="px-6 pt-6 2xl:container">
                    <div class="grid gap-6 md:grid-cols-2 lg:grid-cols-3">
                        <div>
                            <div
                                class="py-6 px-6 rounded-xl border border-gray-200 bg-white"
                            >
                                <h5 class="text-xl text-gray-700">Downloads</h5>
                                <div class="my-8">
                                    <h1
                                        class="text-5xl font-bold text-gray-800"
                                    >
                                        64,5%
                                    </h1>
                                    <span class="text-gray-500"
                                        >Compared to last week $13,988</span
                                    >
                                </div>
                                <svg
                                    class="w-full"
                                    viewBox="0 0 218 69"
                                    fill="none"
                                    xmlns="http://www.w3.org/2000/svg"
                                >
                                    <path
                                        d="M0 67.5C27.8998 67.5 24.6002 15 52.5 15C80.3998 15 77.1002 29 105 29C132.9 29 128.6 52 156.5 52C184.4 52 189.127 63.8158 217.027 63.8158"
                                        stroke="url(#paint0_linear_622:13664)"
                                        stroke-width="3"
                                        stroke-linecap="round"
                                    />
                                    <path
                                        d="M0 67.5C27.2601 67.5 30.7399 31 58 31C85.2601 31 80.7399 2 108 2C135.26 2 134.74 43 162 43C189.26 43 190.74 63.665 218 63.665"
                                        stroke="url(#paint1_linear_622:13664)"
                                        stroke-width="3"
                                        stroke-linecap="round"
                                    />
                                    <defs>
                                        <linearGradient
                                            id="paint0_linear_622:13664"
                                            x1="217.027"
                                            y1="15"
                                            x2="7.91244"
                                            y2="15"
                                            gradientUnits="userSpaceOnUse"
                                        >
                                            <stop stop-color="#4DFFDF" />
                                            <stop
                                                offset="1"
                                                stop-color="#4DA1FF"
                                            />
                                        </linearGradient>
                                        <linearGradient
                                            id="paint1_linear_622:13664"
                                            x1="218"
                                            y1="18.3748"
                                            x2="5.4362"
                                            y2="18.9795"
                                            gradientUnits="userSpaceOnUse"
                                        >
                                            <stop stop-color="#E323FF" />
                                            <stop
                                                offset="1"
                                                stop-color="#7517F8"
                                            />
                                        </linearGradient>
                                    </defs>
                                </svg>
                                <table class="mt-6 -mb-2 w-full text-gray-600">
                                    <tbody>
                                        <tr>
                                            <td class="py-2">From new users</td>
                                            <td class="text-gray-500">896</td>
                                            <td>
                                                <svg
                                                    class="w-16 ml-auto"
                                                    viewBox="0 0 68 21"
                                                    fill="none"
                                                    xmlns="http://www.w3.org/2000/svg"
                                                >
                                                    <rect
                                                        opacity="0.4"
                                                        width="17"
                                                        height="21"
                                                        rx="1"
                                                        fill="#e4e4f2"
                                                    />
                                                    <rect
                                                        opacity="0.4"
                                                        x="19"
                                                        width="14"
                                                        height="21"
                                                        rx="1"
                                                        fill="#e4e4f2"
                                                    />
                                                    <rect
                                                        opacity="0.4"
                                                        x="35"
                                                        width="14"
                                                        height="21"
                                                        rx="1"
                                                        fill="#e4e4f2"
                                                    />
                                                    <rect
                                                        opacity="0.4"
                                                        x="51"
                                                        width="17"
                                                        height="21"
                                                        rx="1"
                                                        fill="#e4e4f2"
                                                    />
                                                    <path
                                                        d="M0 7C8.62687 7 7.61194 16 17.7612 16C27.9104 16 25.3731 9 34 9C42.6269 9 44.5157 5 51.2537 5C57.7936 5 59.3731 14.5 68 14.5"
                                                        stroke="url(#paint0_linear_622:13631)"
                                                        stroke-width="2"
                                                        stroke-linejoin="round"
                                                    />
                                                    <defs>
                                                        <linearGradient
                                                            id="paint0_linear_622:13631"
                                                            x1="68"
                                                            y1="7.74997"
                                                            x2="1.69701"
                                                            y2="8.10029"
                                                            gradientUnits="userSpaceOnUse"
                                                        >
                                                            <stop
                                                                stop-color="#E323FF"
                                                            />
                                                            <stop
                                                                offset="1"
                                                                stop-color="#7517F8"
                                                            />
                                                        </linearGradient>
                                                    </defs>
                                                </svg>
                                            </td>
                                        </tr>
                                        <tr>
                                            <td class="py-2">From old users</td>
                                            <td class="text-gray-500">1200</td>
                                            <td>
                                                <svg
                                                    class="w-16 ml-auto"
                                                    viewBox="0 0 68 21"
                                                    fill="none"
                                                    xmlns="http://www.w3.org/2000/svg"
                                                >
                                                    <rect
                                                        opacity="0.4"
                                                        width="17"
                                                        height="21"
                                                        rx="1"
                                                        fill="#e4e4f2"
                                                    />
                                                    <rect
                                                        opacity="0.4"
                                                        x="19"
                                                        width="14"
                                                        height="21"
                                                        rx="1"
                                                        fill="#e4e4f2"
                                                    />
                                                    <rect
                                                        opacity="0.4"
                                                        x="35"
                                                        width="14"
                                                        height="21"
                                                        rx="1"
                                                        fill="#e4e4f2"
                                                    />
                                                    <rect
                                                        opacity="0.4"
                                                        x="51"
                                                        width="17"
                                                        height="21"
                                                        rx="1"
                                                        fill="#e4e4f2"
                                                    />
                                                    <path
                                                        d="M0 12.929C8.69077 12.929 7.66833 9.47584 17.8928 9.47584C28.1172 9.47584 25.5611 15.9524 34.2519 15.9524C42.9426 15.9524 44.8455 10.929 51.6334 10.929C58.2217 10.929 59.3092 5 68 5"
                                                        stroke="url(#paint0_linear_622:13640)"
                                                        stroke-width="2"
                                                        stroke-linejoin="round"
                                                    />
                                                    <defs>
                                                        <linearGradient
                                                            id="paint0_linear_622:13640"
                                                            x1="34"
                                                            y1="5"
                                                            x2="34"
                                                            y2="15.9524"
                                                            gradientUnits="userSpaceOnUse"
                                                        >
                                                            <stop
                                                                stop-color="#8AFF6C"
                                                            />
                                                            <stop
                                                                offset="1"
                                                                stop-color="#02C751"
                                                            />
                                                        </linearGradient>
                                                    </defs>
                                                </svg>
                                            </td>
                                        </tr>
                                    </tbody>
                                </table>
                            </div>
                        </div>
                        <!-- Tabel two -->
                        <div>
                            <!-- component -->
                            <div
                                class="flex w-full flex-col items-center justify-center gap-y-2"
                            >
                                <div
                                    class="w-[300px] rounded-xl border border-gray-200 bg-white py-4 px-2 shadow-md shadow-gray-100"
                                >
                                    <div
                                        class="flex items-center justify-between px-2 text-base font-medium text-gray-700"
                                    >
                                        <div>Add Block</div>
                                        <div>
                                            <button
                                                class="flex h-8 w-8 items-center justify-center rounded-full bg-gray-200 text-black"
                                            >
                                                <svg
                                                    class="h-5 w-5"
                                                    aria-hidden="true"
                                                    fill="none"
                                                    stroke="currentColor"
                                                    stroke-width="2.5"
                                                    viewBox="0 0 24 24"
                                                    xmlns="http://www.w3.org/2000/svg"
                                                >
                                                    <path
                                                        d="M6 18L18 6M6 6l12 12"
                                                        stroke-linecap="round"
                                                        stroke-linejoin="round"
                                                    ></path>
                                                </svg>
                                            </button>
                                        </div>
                                    </div>
                                    <div class="mt-4">
                                        <div
                                            class="flex max-h-[400px] w-full flex-col overflow-y-scroll"
                                        >
                                            <button
                                                class="group flex items-center gap-x-5 rounded-md px-2.5 py-2 transition-all duration-75 hover:bg-green-100"
                                            >
                                                <div
                                                    class="flex h-12 w-12 items-center rounded-lg bg-gray-200 text-black group-hover:bg-green-200"
                                                >
                                                    <span
                                                        class="tag w-full text-center text-2xl font-medium text-gray-700 group-hover:text-green-900"
                                                        >A</span
                                                    >
                                                </div>
                                                <div
                                                    class="flex flex-col items-start justify-between font-light text-gray-600"
                                                >
                                                    <p class="text-[15px]">
                                                        Text
                                                    </p>
                                                    <span
                                                        class="text-xs font-light text-gray-400"
                                                        >just start writing with
                                                        plain text</span
                                                    >
                                                </div>
                                            </button>
                                            <button
                                                class="group flex items-center gap-x-5 rounded-md px-2.5 py-2 transition-all duration-75 hover:bg-green-100"
                                            >
                                                <div
                                                    class="flex h-12 w-12 items-center rounded-lg bg-gray-200 text-black group-hover:bg-green-200"
                                                >
                                                    <span
                                                        class="tag w-full text-center text-2xl font-medium text-gray-700 group-hover:text-green-900"
                                                    >
                                                        <svg
                                                            class="mx-auto h-6 w-6"
                                                            aria-hidden="true"
                                                            fill="none"
                                                            stroke="currentColor"
                                                            stroke-width="2"
                                                            viewBox="0 0 24 24"
                                                            xmlns="http://www.w3.org/2000/svg"
                                                        >
                                                            <path
                                                                d="M11.35 3.836c-.065.21-.1.433-.1.664 0 .414.336.75.75.75h4.5a.75.75 0 00.75-.75 2.25 2.25 0 00-.1-.664m-5.8 0A2.251 2.251 0 0113.5 2.25H15c1.012 0 1.867.668 2.15 1.586m-5.8 0c-.376.023-.75.05-1.124.08C9.095 4.01 8.25 4.973 8.25 6.108V8.25m8.9-4.414c.376.023.75.05 1.124.08 1.131.094 1.976 1.057 1.976 2.192V16.5A2.25 2.25 0 0118 18.75h-2.25m-7.5-10.5H4.875c-.621 0-1.125.504-1.125 1.125v11.25c0 .621.504 1.125 1.125 1.125h9.75c.621 0 1.125-.504 1.125-1.125V18.75m-7.5-10.5h6.375c.621 0 1.125.504 1.125 1.125v9.375m-8.25-3l1.5 1.5 3-3.75"
                                                                stroke-linecap="round"
                                                                stroke-linejoin="round"
                                                            ></path>
                                                        </svg>
                                                    </span>
                                                </div>
                                                <div
                                                    class="flex flex-col items-start justify-between font-light text-gray-600"
                                                >
                                                    <p class="text-[15px]">
                                                        Checklist
                                                    </p>
                                                    <span
                                                        class="text-xs font-light text-gray-400"
                                                        >create a to-do or
                                                        checklist</span
                                                    >
                                                </div>
                                            </button>
                                            <button
                                                class="group flex items-center gap-x-5 rounded-md px-2.5 py-2 transition-all duration-75 hover:bg-green-100"
                                            >
                                                <div
                                                    class="flex h-12 w-12 items-center rounded-lg bg-gray-200 text-black group-hover:bg-green-200"
                                                >
                                                    <span
                                                        class="tag w-full text-center text-lg font-medium text-gray-700 group-hover:text-green-900"
                                                    >
                                                        H1
                                                    </span>
                                                </div>
                                                <div
                                                    class="flex flex-col items-start justify-between font-light text-gray-600"
                                                >
                                                    <p class="text-[15px]">
                                                        Heading 1
                                                    </p>
                                                    <span
                                                        class="text-xs font-light text-gray-400"
                                                        >Big section
                                                        heading</span
                                                    >
                                                </div>
                                            </button>
                                            <button
                                                class="group flex items-center gap-x-5 rounded-md px-2.5 py-2 transition-all duration-75 hover:bg-green-100"
                                            >
                                                <div
                                                    class="flex h-12 w-12 items-center rounded-lg bg-gray-200 text-black group-hover:bg-green-200"
                                                >
                                                    <span
                                                        class="tag w-full text-center text-lg font-medium text-gray-700 group-hover:text-green-900"
                                                    >
                                                        H2
                                                    </span>
                                                </div>
                                                <div
                                                    class="flex flex-col items-start justify-between font-light text-gray-600"
                                                >
                                                    <p class="text-[15px]">
                                                        Heading 2
                                                    </p>
                                                    <span
                                                        class="text-xs font-light text-gray-400"
                                                        >Medium section
                                                        heading</span
                                                    >
                                                </div>
                                            </button>
                                            <button
                                                class="group flex items-center gap-x-5 rounded-md px-2.5 py-2 transition-all duration-75 hover:bg-green-100"
                                            >
                                                <div
                                                    class="flex h-12 w-12 items-center rounded-lg bg-gray-200 text-black group-hover:bg-green-200"
                                                >
                                                    <span
                                                        class="tag w-full text-center text-lg font-medium text-gray-700 group-hover:text-green-900"
                                                    >
                                                        H3
                                                    </span>
                                                </div>
                                                <div
                                                    class="flex flex-col items-start justify-between font-light text-gray-600"
                                                >
                                                    <p class="text-[15px]">
                                                        Heading 3
                                                    </p>
                                                    <span
                                                        class="text-xs font-light text-gray-400"
                                                        >small section
                                                        heading</span
                                                    >
                                                </div>
                                            </button>
                                            <h3
                                                class="my-2 px-4 text-[15px] text-gray-400"
                                            >
                                                More
                                            </h3>
                                            <button
                                                class="group flex items-center gap-x-5 rounded-md px-2.5 py-2 transition-all duration-75 hover:bg-green-100"
                                            >
                                                <div
                                                    class="flex h-12 w-12 items-center rounded-lg bg-gray-200 text-black group-hover:bg-green-200"
                                                >
                                                    <span
                                                        class="tag w-full text-center text-xl font-medium text-gray-700 group-hover:text-green-900"
                                                    >
                                                        <svg
                                                            class="mx-auto h-6 w-6"
                                                            aria-hidden="true"
                                                            fill="none"
                                                            stroke="currentColor"
                                                            stroke-width="2"
                                                            viewBox="0 0 24 24"
                                                            xmlns="http://www.w3.org/2000/svg"
                                                        >
                                                            <path
                                                                d="M8.25 6.75h12M8.25 12h12m-12 5.25h12M3.75 6.75h.007v.008H3.75V6.75zm.375 0a.375.375 0 11-.75 0 .375.375 0 01.75 0zM3.75 12h.007v.008H3.75V12zm.375 0a.375.375 0 11-.75 0 .375.375 0 01.75 0zm-.375 5.25h.007v.008H3.75v-.008zm.375 0a.375.375 0 11-.75 0 .375.375 0 01.75 0z"
                                                                stroke-linecap="round"
                                                                stroke-linejoin="round"
                                                            ></path>
                                                        </svg>
                                                    </span>
                                                </div>
                                                <div
                                                    class="flex flex-col items-start justify-between font-light text-gray-600"
                                                >
                                                    <p class="text-[15px]">
                                                        Bullet list
                                                    </p>
                                                    <span
                                                        class="text-xs font-light text-gray-400"
                                                        >Create a simple bullet
                                                        list</span
                                                    >
                                                </div>
                                            </button>
                                            <button
                                                class="group flex items-center gap-x-5 rounded-md px-2.5 py-2 transition-all duration-75 hover:bg-green-100"
                                            >
                                                <div
                                                    class="flex h-12 w-12 items-center rounded-lg bg-gray-200 text-black group-hover:bg-green-200"
                                                >
                                                    <span
                                                        class="tag w-full text-center text-xl font-medium text-gray-700 group-hover:text-green-900"
                                                    >
                                                        <svg
                                                            class="mx-auto h-6 w-6"
                                                            width="100%"
                                                            height="100%"
                                                            viewBox="0 0 24 24"
                                                        >
                                                            <g
                                                                fill="currentColor"
                                                                fill-rule="evenodd"
                                                            >
                                                                <path
                                                                    d="M21 16a1 1 0 0 1 0 2H10a1 1 0 0 1 0-2h11zm0-10a1 1 0 0 1 0 2H10a1 1 0 1 1 0-2h11z"
                                                                ></path>
                                                                <path
                                                                    d="M4.464 13.74c.256 0 .496.036.72.108.224.072.419.179.584.32.165.141.295.319.388.532.093.213.14.461.14.744 0 .181-.019.345-.056.492a1.666 1.666 0 0 1-.392.732c-.09.101-.19.2-.296.296l-1.72 1.48h2.512V19.5H2.392v-1.272l2.2-1.976c.112-.101.224-.216.336-.344a.66.66 0 0 0 .168-.448.544.544 0 0 0-.208-.452.765.765 0 0 0-.488-.164c-.224 0-.399.07-.524.208a.839.839 0 0 0-.212.512l-1.2-.088c.016-.293.077-.548.184-.764.107-.216.248-.396.424-.54.176-.144.383-.252.62-.324.237-.072.495-.108.772-.108zm.992-9.404V10H4.304V5.68l-1.136 1-.68-.784 1.848-1.56h1.12z"
                                                                ></path>
                                                            </g>
                                                        </svg>
                                                    </span>
                                                </div>
                                                <div
                                                    class="flex flex-col items-start justify-between font-light text-gray-600"
                                                >
                                                    <p class="text-[15px]">
                                                        Ordered list
                                                    </p>
                                                    <span
                                                        class="text-xs font-light text-gray-400"
                                                        >Create a list with
                                                        numbered</span
                                                    >
                                                </div>
                                            </button>
                                            <button
                                                class="group flex items-center gap-x-5 rounded-md px-2.5 py-2 transition-all duration-75 hover:bg-green-100"
                                            >
                                                <div
                                                    class="flex h-12 w-12 items-center rounded-lg bg-gray-200 text-black group-hover:bg-green-200"
                                                >
                                                    <span
                                                        class="tag w-full text-center text-xl font-medium text-gray-700 group-hover:text-green-900"
                                                    >
                                                        <svg
                                                            class="mx-auto h-6 w-6"
                                                            aria-hidden="true"
                                                            fill="none"
                                                            stroke="currentColor"
                                                            stroke-width="2"
                                                            viewBox="0 0 24 24"
                                                            xmlns="http://www.w3.org/2000/svg"
                                                        >
                                                            <path
                                                                d="M11.25 11.25l.041-.02a.75.75 0 011.063.852l-.708 2.836a.75.75 0 001.063.853l.041-.021M21 12a9 9 0 11-18 0 9 9 0 0118 0zm-9-3.75h.008v.008H12V8.25z"
                                                                stroke-linecap="round"
                                                                stroke-linejoin="round"
                                                            ></path>
                                                        </svg>
                                                    </span>
                                                </div>
                                                <div
                                                    class="flex flex-col items-start justify-between font-light text-gray-600"
                                                >
                                                    <p class="text-[15px]">
                                                        Info box
                                                    </p>
                                                    <span
                                                        class="text-xs font-light text-gray-400"
                                                        >Add a box with
                                                        additional info</span
                                                    >
                                                </div>
                                            </button>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>

                        <!-- table three -->
                        <div>
                            <!-- component -->
                            <div
                                class="flex w-full flex-col items-center justify-center gap-y-2"
                            >
                                <div
                                    class="w-[300px] rounded-xl border border-gray-200 bg-white py-4 px-2 shadow-md shadow-gray-100"
                                >
                                    <div
                                        class="flex items-center justify-between px-2 text-base font-medium text-gray-700"
                                    >
                                        <div>Add Block</div>
                                        <div>
                                            <button
                                                class="flex h-8 w-8 items-center justify-center rounded-full bg-gray-200 text-black"
                                            >
                                                <svg
                                                    class="h-5 w-5"
                                                    aria-hidden="true"
                                                    fill="none"
                                                    stroke="currentColor"
                                                    stroke-width="2.5"
                                                    viewBox="0 0 24 24"
                                                    xmlns="http://www.w3.org/2000/svg"
                                                >
                                                    <path
                                                        d="M6 18L18 6M6 6l12 12"
                                                        stroke-linecap="round"
                                                        stroke-linejoin="round"
                                                    ></path>
                                                </svg>
                                            </button>
                                        </div>
                                    </div>
                                    <div class="mt-4">
                                        <div
                                            class="flex max-h-[400px] w-full flex-col overflow-y-scroll"
                                        >
                                            <button
                                                class="group flex items-center gap-x-5 rounded-md px-2.5 py-2 transition-all duration-75 hover:bg-green-100"
                                            >
                                                <div
                                                    class="flex h-12 w-12 items-center rounded-lg bg-gray-200 text-black group-hover:bg-green-200"
                                                >
                                                    <span
                                                        class="tag w-full text-center text-2xl font-medium text-gray-700 group-hover:text-green-900"
                                                        >A</span
                                                    >
                                                </div>
                                                <div
                                                    class="flex flex-col items-start justify-between font-light text-gray-600"
                                                >
                                                    <p class="text-[15px]">
                                                        Text
                                                    </p>
                                                    <span
                                                        class="text-xs font-light text-gray-400"
                                                        >just start writing with
                                                        plain text</span
                                                    >
                                                </div>
                                            </button>
                                            <button
                                                class="group flex items-center gap-x-5 rounded-md px-2.5 py-2 transition-all duration-75 hover:bg-green-100"
                                            >
                                                <div
                                                    class="flex h-12 w-12 items-center rounded-lg bg-gray-200 text-black group-hover:bg-green-200"
                                                >
                                                    <span
                                                        class="tag w-full text-center text-2xl font-medium text-gray-700 group-hover:text-green-900"
                                                    >
                                                        <svg
                                                            class="mx-auto h-6 w-6"
                                                            aria-hidden="true"
                                                            fill="none"
                                                            stroke="currentColor"
                                                            stroke-width="2"
                                                            viewBox="0 0 24 24"
                                                            xmlns="http://www.w3.org/2000/svg"
                                                        >
                                                            <path
                                                                d="M11.35 3.836c-.065.21-.1.433-.1.664 0 .414.336.75.75.75h4.5a.75.75 0 00.75-.75 2.25 2.25 0 00-.1-.664m-5.8 0A2.251 2.251 0 0113.5 2.25H15c1.012 0 1.867.668 2.15 1.586m-5.8 0c-.376.023-.75.05-1.124.08C9.095 4.01 8.25 4.973 8.25 6.108V8.25m8.9-4.414c.376.023.75.05 1.124.08 1.131.094 1.976 1.057 1.976 2.192V16.5A2.25 2.25 0 0118 18.75h-2.25m-7.5-10.5H4.875c-.621 0-1.125.504-1.125 1.125v11.25c0 .621.504 1.125 1.125 1.125h9.75c.621 0 1.125-.504 1.125-1.125V18.75m-7.5-10.5h6.375c.621 0 1.125.504 1.125 1.125v9.375m-8.25-3l1.5 1.5 3-3.75"
                                                                stroke-linecap="round"
                                                                stroke-linejoin="round"
                                                            ></path>
                                                        </svg>
                                                    </span>
                                                </div>
                                                <div
                                                    class="flex flex-col items-start justify-between font-light text-gray-600"
                                                >
                                                    <p class="text-[15px]">
                                                        Checklist
                                                    </p>
                                                    <span
                                                        class="text-xs font-light text-gray-400"
                                                        >create a to-do or
                                                        checklist</span
                                                    >
                                                </div>
                                            </button>
                                            <button
                                                class="group flex items-center gap-x-5 rounded-md px-2.5 py-2 transition-all duration-75 hover:bg-green-100"
                                            >
                                                <div
                                                    class="flex h-12 w-12 items-center rounded-lg bg-gray-200 text-black group-hover:bg-green-200"
                                                >
                                                    <span
                                                        class="tag w-full text-center text-lg font-medium text-gray-700 group-hover:text-green-900"
                                                    >
                                                        H1
                                                    </span>
                                                </div>
                                                <div
                                                    class="flex flex-col items-start justify-between font-light text-gray-600"
                                                >
                                                    <p class="text-[15px]">
                                                        Heading 1
                                                    </p>
                                                    <span
                                                        class="text-xs font-light text-gray-400"
                                                        >Big section
                                                        heading</span
                                                    >
                                                </div>
                                            </button>
                                            <button
                                                class="group flex items-center gap-x-5 rounded-md px-2.5 py-2 transition-all duration-75 hover:bg-green-100"
                                            >
                                                <div
                                                    class="flex h-12 w-12 items-center rounded-lg bg-gray-200 text-black group-hover:bg-green-200"
                                                >
                                                    <span
                                                        class="tag w-full text-center text-lg font-medium text-gray-700 group-hover:text-green-900"
                                                    >
                                                        H2
                                                    </span>
                                                </div>
                                                <div
                                                    class="flex flex-col items-start justify-between font-light text-gray-600"
                                                >
                                                    <p class="text-[15px]">
                                                        Heading 2
                                                    </p>
                                                    <span
                                                        class="text-xs font-light text-gray-400"
                                                        >Medium section
                                                        heading</span
                                                    >
                                                </div>
                                            </button>
                                            <button
                                                class="group flex items-center gap-x-5 rounded-md px-2.5 py-2 transition-all duration-75 hover:bg-green-100"
                                            >
                                                <div
                                                    class="flex h-12 w-12 items-center rounded-lg bg-gray-200 text-black group-hover:bg-green-200"
                                                >
                                                    <span
                                                        class="tag w-full text-center text-lg font-medium text-gray-700 group-hover:text-green-900"
                                                    >
                                                        H3
                                                    </span>
                                                </div>
                                                <div
                                                    class="flex flex-col items-start justify-between font-light text-gray-600"
                                                >
                                                    <p class="text-[15px]">
                                                        Heading 3
                                                    </p>
                                                    <span
                                                        class="text-xs font-light text-gray-400"
                                                        >small section
                                                        heading</span
                                                    >
                                                </div>
                                            </button>
                                            <h3
                                                class="my-2 px-4 text-[15px] text-gray-400"
                                            >
                                                More
                                            </h3>
                                            <button
                                                class="group flex items-center gap-x-5 rounded-md px-2.5 py-2 transition-all duration-75 hover:bg-green-100"
                                            >
                                                <div
                                                    class="flex h-12 w-12 items-center rounded-lg bg-gray-200 text-black group-hover:bg-green-200"
                                                >
                                                    <span
                                                        class="tag w-full text-center text-xl font-medium text-gray-700 group-hover:text-green-900"
                                                    >
                                                        <svg
                                                            class="mx-auto h-6 w-6"
                                                            aria-hidden="true"
                                                            fill="none"
                                                            stroke="currentColor"
                                                            stroke-width="2"
                                                            viewBox="0 0 24 24"
                                                            xmlns="http://www.w3.org/2000/svg"
                                                        >
                                                            <path
                                                                d="M8.25 6.75h12M8.25 12h12m-12 5.25h12M3.75 6.75h.007v.008H3.75V6.75zm.375 0a.375.375 0 11-.75 0 .375.375 0 01.75 0zM3.75 12h.007v.008H3.75V12zm.375 0a.375.375 0 11-.75 0 .375.375 0 01.75 0zm-.375 5.25h.007v.008H3.75v-.008zm.375 0a.375.375 0 11-.75 0 .375.375 0 01.75 0z"
                                                                stroke-linecap="round"
                                                                stroke-linejoin="round"
                                                            ></path>
                                                        </svg>
                                                    </span>
                                                </div>
                                                <div
                                                    class="flex flex-col items-start justify-between font-light text-gray-600"
                                                >
                                                    <p class="text-[15px]">
                                                        Bullet list
                                                    </p>
                                                    <span
                                                        class="text-xs font-light text-gray-400"
                                                        >Create a simple bullet
                                                        list</span
                                                    >
                                                </div>
                                            </button>
                                            <button
                                                class="group flex items-center gap-x-5 rounded-md px-2.5 py-2 transition-all duration-75 hover:bg-green-100"
                                            >
                                                <div
                                                    class="flex h-12 w-12 items-center rounded-lg bg-gray-200 text-black group-hover:bg-green-200"
                                                >
                                                    <span
                                                        class="tag w-full text-center text-xl font-medium text-gray-700 group-hover:text-green-900"
                                                    >
                                                        <svg
                                                            class="mx-auto h-6 w-6"
                                                            width="100%"
                                                            height="100%"
                                                            viewBox="0 0 24 24"
                                                        >
                                                            <g
                                                                fill="currentColor"
                                                                fill-rule="evenodd"
                                                            >
                                                                <path
                                                                    d="M21 16a1 1 0 0 1 0 2H10a1 1 0 0 1 0-2h11zm0-10a1 1 0 0 1 0 2H10a1 1 0 1 1 0-2h11z"
                                                                ></path>
                                                                <path
                                                                    d="M4.464 13.74c.256 0 .496.036.72.108.224.072.419.179.584.32.165.141.295.319.388.532.093.213.14.461.14.744 0 .181-.019.345-.056.492a1.666 1.666 0 0 1-.392.732c-.09.101-.19.2-.296.296l-1.72 1.48h2.512V19.5H2.392v-1.272l2.2-1.976c.112-.101.224-.216.336-.344a.66.66 0 0 0 .168-.448.544.544 0 0 0-.208-.452.765.765 0 0 0-.488-.164c-.224 0-.399.07-.524.208a.839.839 0 0 0-.212.512l-1.2-.088c.016-.293.077-.548.184-.764.107-.216.248-.396.424-.54.176-.144.383-.252.62-.324.237-.072.495-.108.772-.108zm.992-9.404V10H4.304V5.68l-1.136 1-.68-.784 1.848-1.56h1.12z"
                                                                ></path>
                                                            </g>
                                                        </svg>
                                                    </span>
                                                </div>
                                                <div
                                                    class="flex flex-col items-start justify-between font-light text-gray-600"
                                                >
                                                    <p class="text-[15px]">
                                                        Ordered list
                                                    </p>
                                                    <span
                                                        class="text-xs font-light text-gray-400"
                                                        >Create a list with
                                                        numbered</span
                                                    >
                                                </div>
                                            </button>
                                            <button
                                                class="group flex items-center gap-x-5 rounded-md px-2.5 py-2 transition-all duration-75 hover:bg-green-100"
                                            >
                                                <div
                                                    class="flex h-12 w-12 items-center rounded-lg bg-gray-200 text-black group-hover:bg-green-200"
                                                >
                                                    <span
                                                        class="tag w-full text-center text-xl font-medium text-gray-700 group-hover:text-green-900"
                                                    >
                                                        <svg
                                                            class="mx-auto h-6 w-6"
                                                            aria-hidden="true"
                                                            fill="none"
                                                            stroke="currentColor"
                                                            stroke-width="2"
                                                            viewBox="0 0 24 24"
                                                            xmlns="http://www.w3.org/2000/svg"
                                                        >
                                                            <path
                                                                d="M11.25 11.25l.041-.02a.75.75 0 011.063.852l-.708 2.836a.75.75 0 001.063.853l.041-.021M21 12a9 9 0 11-18 0 9 9 0 0118 0zm-9-3.75h.008v.008H12V8.25z"
                                                                stroke-linecap="round"
                                                                stroke-linejoin="round"
                                                            ></path>
                                                        </svg>
                                                    </span>
                                                </div>
                                                <div
                                                    class="flex flex-col items-start justify-between font-light text-gray-600"
                                                >
                                                    <p class="text-[15px]">
                                                        Info box
                                                    </p>
                                                    <span
                                                        class="text-xs font-light text-gray-400"
                                                        >Add a box with
                                                        additional info</span
                                                    >
                                                </div>
                                            </button>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <div>
                    <!-- Main Tablecomponent -->
                    <div
                        class="-my-2 py-2 overflow-x-auto sm:-mx-6 sm:px-6 lg:-mx-8 pr-10 lg:px-8"
                    >
                        <div
                            class="align-middle rounded-tl-lg rounded-tr-lg inline-block w-full py-4 overflow-hidden bg-white shadow-lg px-12"
                        >
                            <div class="flex justify-between">
                                <div
                                    class="inline-flex border rounded w-7/12 px-2 lg:px-6 h-12 bg-transparent"
                                >
                                    <div
                                        class="flex flex-wrap items-stretch w-full h-full mb-6 relative"
                                    >
                                        <div class="flex">
                                            <span
                                                class="flex items-center leading-normal bg-transparent rounded rounded-r-none border border-r-0 border-none lg:px-3 py-2 whitespace-no-wrap text-grey-dark text-sm"
                                            >
                                                <svg
                                                    width="18"
                                                    height="18"
                                                    class="w-4 lg:w-auto"
                                                    viewBox="0 0 18 18"
                                                    fill="none"
                                                    xmlns="http://www.w3.org/2000/svg"
                                                >
                                                    <path
                                                        d="M8.11086 15.2217C12.0381 15.2217 15.2217 12.0381 15.2217 8.11086C15.2217 4.18364 12.0381 1 8.11086 1C4.18364 1 1 4.18364 1 8.11086C1 12.0381 4.18364 15.2217 8.11086 15.2217Z"
                                                        stroke="#455A64"
                                                        stroke-linecap="round"
                                                        stroke-linejoin="round"
                                                    />
                                                    <path
                                                        d="M16.9993 16.9993L13.1328 13.1328"
                                                        stroke="#455A64"
                                                        stroke-linecap="round"
                                                        stroke-linejoin="round"
                                                    />
                                                </svg>
                                            </span>
                                        </div>
                                        <input
                                            type="text"
                                            class="flex-shrink flex-grow flex-auto leading-normal tracking-wide w-px flex-1 border border-none border-l-0 rounded rounded-l-none px-3 relative focus:outline-none text-xxs lg:text-xs lg:text-base text-gray-500 font-thin"
                                            placeholder="Search"
                                        />
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div
                            class="align-middle inline-block min-w-full shadow overflow-hidden bg-white shadow-dashboard px-8 pt-3 rounded-bl-lg rounded-br-lg"
                        >
                            <table class="min-w-full">
                                <thead>
                                    <tr>
                                        <th
                                            class="px-6 py-3 border-b-2 border-gray-300 text-left leading-4 text-blue-500 tracking-wider"
                                        >
                                            ID
                                        </th>
                                        <th
                                            class="px-6 py-3 border-b-2 border-gray-300 text-left text-sm leading-4 text-blue-500 tracking-wider"
                                        >
                                            Fullname
                                        </th>
                                        <th
                                            class="px-6 py-3 border-b-2 border-gray-300 text-left text-sm leading-4 text-blue-500 tracking-wider"
                                        >
                                            Email
                                        </th>
                                        <th
                                            class="px-6 py-3 border-b-2 border-gray-300 text-left text-sm leading-4 text-blue-500 tracking-wider"
                                        >
                                            Phone
                                        </th>
                                        <th
                                            class="px-6 py-3 border-b-2 border-gray-300 text-left text-sm leading-4 text-blue-500 tracking-wider"
                                        >
                                            Status
                                        </th>
                                        <th
                                            class="px-6 py-3 border-b-2 border-gray-300 text-left text-sm leading-4 text-blue-500 tracking-wider"
                                        >
                                            Created
                                        </th>
                                        <th
                                            class="px-6 py-3 border-b-2 border-gray-300"
                                        ></th>
                                    </tr>
                                </thead>
                                <tbody class="bg-white">
                                    <tr>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b border-gray-500"
                                        >
                                            <div class="flex items-center">
                                                <div>
                                                    <div
                                                        class="text-sm leading-5 text-gray-800"
                                                    >
                                                        #1
                                                    </div>
                                                </div>
                                            </div>
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b border-gray-500"
                                        >
                                            <div
                                                class="text-sm leading-5 text-blue-900"
                                            >
                                                Damilare Anjorin
                                            </div>
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b text-blue-900 border-gray-500 text-sm leading-5"
                                        >
                                            damilareanjorin1@gmail.com
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b text-blue-900 border-gray-500 text-sm leading-5"
                                        >
                                            +2348106420637
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b text-blue-900 border-gray-500 text-sm leading-5"
                                        >
                                            <span
                                                class="relative inline-block px-3 py-1 font-semibold text-green-900 leading-tight"
                                            >
                                                <span
                                                    aria-hidden
                                                    class="absolute inset-0 bg-green-200 opacity-50 rounded-full"
                                                ></span>
                                                <span class="relative text-xs"
                                                    >active</span
                                                >
                                            </span>
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b border-gray-500 text-blue-900 text-sm leading-5"
                                        >
                                            September 12
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap text-right border-b border-gray-500 text-sm leading-5"
                                        >
                                            <button
                                                class="px-5 py-2 border-blue-500 border text-blue-500 rounded transition duration-300 hover:bg-blue-700 hover:text-white focus:outline-none"
                                            >
                                                View
                                            </button>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b border-gray-500"
                                        >
                                            <div class="flex items-center">
                                                <div>
                                                    <div
                                                        class="text-sm leading-5 text-gray-800"
                                                    >
                                                        #1
                                                    </div>
                                                </div>
                                            </div>
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b border-gray-500"
                                        >
                                            <div
                                                class="text-sm leading-5 text-blue-900"
                                            >
                                                Damilare Anjorin
                                            </div>
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b text-blue-900 border-gray-500 text-sm leading-5"
                                        >
                                            damilareanjorin1@gmail.com
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b text-blue-900 border-gray-500 text-sm leading-5"
                                        >
                                            +2348106420637
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b text-blue-900 border-gray-500 text-sm leading-5"
                                        >
                                            <span
                                                class="relative inline-block px-3 py-1 font-semibold text-green-900 leading-tight"
                                            >
                                                <span
                                                    aria-hidden
                                                    class="absolute inset-0 bg-green-200 opacity-50 rounded-full"
                                                ></span>
                                                <span class="relative text-xs"
                                                    >active</span
                                                >
                                            </span>
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b border-gray-500 text-blue-900 text-sm leading-5"
                                        >
                                            September 12
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap text-right border-b border-gray-500 text-sm leading-5"
                                        >
                                            <button
                                                class="px-5 py-2 border-blue-500 border text-blue-500 rounded transition duration-300 hover:bg-blue-700 hover:text-white focus:outline-none"
                                            >
                                                View
                                            </button>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b border-gray-500"
                                        >
                                            <div class="flex items-center">
                                                <div>
                                                    <div
                                                        class="text-sm leading-5 text-gray-800"
                                                    >
                                                        #1
                                                    </div>
                                                </div>
                                            </div>
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b border-gray-500"
                                        >
                                            <div
                                                class="text-sm leading-5 text-blue-900"
                                            >
                                                Damilare Anjorin
                                            </div>
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b text-blue-900 border-gray-500 text-sm leading-5"
                                        >
                                            damilareanjorin1@gmail.com
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b text-blue-900 border-gray-500 text-sm leading-5"
                                        >
                                            +2348106420637
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b text-blue-900 border-gray-500 text-sm leading-5"
                                        >
                                            <span
                                                class="relative inline-block px-3 py-1 font-semibold text-red-900 leading-tight"
                                            >
                                                <span
                                                    aria-hidden
                                                    class="absolute inset-0 bg-red-200 opacity-50 rounded-full"
                                                ></span>
                                                <span class="relative text-xs"
                                                    >cancle</span
                                                >
                                            </span>
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b border-gray-500 text-blue-900 text-sm leading-5"
                                        >
                                            September 12
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap text-right border-b border-gray-500 text-sm leading-5"
                                        >
                                            <button
                                                class="px-5 py-2 border-blue-500 border text-blue-500 rounded transition duration-300 hover:bg-blue-700 hover:text-white focus:outline-none"
                                            >
                                                View
                                            </button>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b border-gray-500"
                                        >
                                            <div class="flex items-center">
                                                <div>
                                                    <div
                                                        class="text-sm leading-5 text-gray-800"
                                                    >
                                                        #1
                                                    </div>
                                                </div>
                                            </div>
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b border-gray-500"
                                        >
                                            <div
                                                class="text-sm leading-5 text-blue-900"
                                            >
                                                Damilare Anjorin
                                            </div>
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b text-blue-900 border-gray-500 text-sm leading-5"
                                        >
                                            damilareanjorin1@gmail.com
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b text-blue-900 border-gray-500 text-sm leading-5"
                                        >
                                            +2348106420637
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b text-blue-900 border-gray-500 text-sm leading-5"
                                        >
                                            <span
                                                class="relative inline-block px-3 py-1 font-semibold text-green-900 leading-tight"
                                            >
                                                <span
                                                    aria-hidden
                                                    class="absolute inset-0 bg-green-200 opacity-50 rounded-full"
                                                ></span>
                                                <span class="relative text-xs"
                                                    >active</span
                                                >
                                            </span>
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b border-gray-500 text-blue-900 text-sm leading-5"
                                        >
                                            September 12
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap text-right border-b border-gray-500 text-sm leading-5"
                                        >
                                            <button
                                                class="px-5 py-2 border-blue-500 border text-blue-500 rounded transition duration-300 hover:bg-blue-700 hover:text-white focus:outline-none"
                                            >
                                                View
                                            </button>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b border-gray-500"
                                        >
                                            <div class="flex items-center">
                                                <div>
                                                    <div
                                                        class="text-sm leading-5 text-gray-800"
                                                    >
                                                        #1
                                                    </div>
                                                </div>
                                            </div>
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b border-gray-500"
                                        >
                                            <div
                                                class="text-sm leading-5 text-blue-900"
                                            >
                                                Damilare Anjorin
                                            </div>
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b text-blue-900 border-gray-500 text-sm leading-5"
                                        >
                                            damilareanjorin1@gmail.com
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b text-blue-900 border-gray-500 text-sm leading-5"
                                        >
                                            +2348106420637
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b text-blue-900 border-gray-500 text-sm leading-5"
                                        >
                                            <span
                                                class="relative inline-block px-3 py-1 font-semibold text-orange-900 leading-tight"
                                            >
                                                <span
                                                    aria-hidden
                                                    class="absolute inset-0 bg-orange-200 opacity-50 rounded-full"
                                                ></span>
                                                <span class="relative text-xs"
                                                    >disabled</span
                                                >
                                            </span>
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap border-b border-gray-500 text-blue-900 text-sm leading-5"
                                        >
                                            September 12
                                        </td>
                                        <td
                                            class="px-6 py-4 whitespace-no-wrap text-right border-b border-gray-500 text-sm leading-5"
                                        >
                                            <button
                                                class="px-5 py-2 border-blue-500 border text-blue-500 rounded transition duration-300 hover:bg-blue-700 hover:text-white focus:outline-none"
                                            >
                                                View
                                            </button>
                                        </td>
                                    </tr>
                                </tbody>
                            </table>
                            <div
                                class="sm:flex-1 sm:flex sm:items-center sm:justify-between mt-4 work-sans"
                            >
                                <div>
                                    <p class="text-sm leading-5 text-blue-700">
                                        Showing
                                        <span class="font-medium">1</span>
                                        to
                                        <span class="font-medium">200</span>
                                        of
                                        <span class="font-medium">2000</span>
                                        results
                                    </p>
                                </div>
                                <div></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </AdminLayout>
</template>
