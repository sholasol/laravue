<script setup>
import AdminLayout from "@/Layouts/AdminLayout.vue";
import { Head, Link } from "@inertiajs/vue3";
import Table from "@/Components/Table.vue";
import TableData from "@/Components/TableData.vue";
import TableHeader from "@/Components/TableHeader.vue";
import TableRow from "@/Components/TableRow.vue";

defineProps(["permissions"]);
</script>

<template>
    <Head title="Permissions" />

    <AdminLayout>
        <div class="flex justify-between">
            <h2 class="font-semibold text-xl text-gray-800 leading-tight">
                Permissions
            </h2>
            <Link
                :href="route('permissions.create')"
                class="px-3 py-2 text-white font-semibold bg-indigo-500 hover:bg-indigo-700 rounded"
            >
                Add Permission
            </Link>
        </div>

        <div class="py-4">
            <Table>
                <template #header>
                    <TableRow>
                        <TableHeader width="5%">ID</TableHeader>
                        <TableHeader>Name</TableHeader>
                        <TableHeader width="15%">Action</TableHeader>
                    </TableRow>
                </template>
                <template #default>
                    <TableRow
                        v-for="permission in permissions"
                        :key="permission.id"
                        class="border-b"
                    >
                        <TableData> {{ permission.id }}</TableData>
                        <TableData> {{ permission.name }}</TableData>
                        <TableData>
                            <Link
                                :href="route('permissions.edit', permission.id)"
                                type="button"
                                class="btn-sm text-white bg-green-700 hover:bg-green-800 focus:ring-4 focus:outline-none focus:ring-green-300 font-medium rounded-full text-sm p-2.5 text-center inline-flex items-center mr-2 dark:bg-green-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
                            >
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
                                        d="M16.862 4.487l1.687-1.688a1.875 1.875 0 112.652 2.652L10.582 16.07a4.5 4.5 0 01-1.897 1.13L6 18l.8-2.685a4.5 4.5 0 011.13-1.897l8.932-8.931zm0 0L19.5 7.125M18 14v4.75A2.25 2.25 0 0115.75 21H5.25A2.25 2.25 0 013 18.75V8.25A2.25 2.25 0 015.25 6H10"
                                    />
                                </svg>

                                <span class="sr-only">Icon description</span>
                            </Link>
                            <Link
                                :href="
                                    route('permissions.destroy', permission.id)
                                "
                                method="DELETE"
                                as="button"
                                class="btn-sm text-white bg-blue-700 hover:bg-red-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-full text-sm p-2.5 text-center inline-flex items-center mr-2 dark:bg-red-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
                            >
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
                                        d="M14.74 9l-.346 9m-4.788 0L9.26 9m9.968-3.21c.342.052.682.107 1.022.166m-1.022-.165L18.16 19.673a2.25 2.25 0 01-2.244 2.077H8.084a2.25 2.25 0 01-2.244-2.077L4.772 5.79m14.456 0a48.108 48.108 0 00-3.478-.397m-12 .562c.34-.059.68-.114 1.022-.165m0 0a48.11 48.11 0 013.478-.397m7.5 0v-.916c0-1.18-.91-2.164-2.09-2.201a51.964 51.964 0 00-3.32 0c-1.18.037-2.09 1.022-2.09 2.201v.916m7.5 0a48.667 48.667 0 00-7.5 0"
                                    />
                                </svg>

                                <span class="sr-only">Icon description</span>
                            </Link>
                        </TableData>
                    </TableRow>
                </template>
            </Table>
        </div>
    </AdminLayout>
</template>
