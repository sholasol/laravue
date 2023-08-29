<script setup>
import AdminLayout from "@/Layouts/AdminLayout.vue";
import { Head, Link, useForm } from "@inertiajs/vue3";
import PrimaryButton from "@/Components/PrimaryButton.vue";
import InputLabel from "@/Components/InputLabel.vue";
import InputError from "@/Components/InputError.vue";
import TextInput from "@/Components/TextInput.vue";
import VueMultiselect from "vue-multiselect";
import Table from "@/Components/Table.vue";
import TableData from "@/Components/TableData.vue";
import TableHeader from "@/Components/TableHeader.vue";
import TableRow from "@/Components/TableRow.vue";
import { onMounted, watch } from "vue";

const props = defineProps({
    role: {
        type: Object,
        required: true,
    },
    permissions: Array,
});

const form = useForm({
    name: props.role.name,
    permissions: [],
});

onMounted(() => {
    form.permissions = props.role.permissions;
});

watch(
    () => props.role,
    () => (form.permissions = props.role?.permissions)
);
</script>

<template>
    <Head title="Create Roles" />

    <AdminLayout>
        <div class="max-w-12xl mx-auto py-4">
            <div class="flex justify-between">
                <h2 class="font-semibold text-xl text-gray-800 leading-tight">
                    Update Roles 1
                </h2>
                <Link
                    :href="route('roles.index')"
                    class="px-3 py-2 text-white font-semibold bg-indigo-500 hover:bg-indigo-700 rounded"
                >
                    Back
                </Link>
            </div>

            <div class="mt-6 max-w-2xl mx-auto bg-slate-100 shadow-lg p-6">
                <h2 class="text-2xl font-semibold text-indigo-700 mb-2">
                    Add Permission to Role
                </h2>
                <form
                    @submit.prevent="form.put(route('roles.update', role.id))"
                >
                    <div class="mt-4">
                        <InputLabel for="name" value="Name" />

                        <TextInput
                            id="name"
                            type="name"
                            v-model="form.name"
                            class="mt-1 block w-full border-b"
                            autofocus
                            autocomplete="name"
                        />

                        <InputError class="mt-2" :message="form.errors.name" />
                    </div>
                    <div class="mt-4">
                        <InputLabel for="permissons" value="Permissions" />
                        <VueMultiselect
                            v-model="form.permissions"
                            :options="permissions"
                            :multiple="true"
                            :close-on-select="true"
                            placeholder="Pick some"
                            label="name"
                            track-by="id"
                        />
                    </div>

                    <div class="flex items-center mt-4">
                        <PrimaryButton class="ml-4"> Update </PrimaryButton>
                    </div>
                </form>
            </div>

            <div class="mt-6 max-w-2xl mx-auto bg-slate-100 shadow-lg p-6">
                <h2 class="text-2xl font-semibold text-indigo-700 mb-2">
                    Permissions
                </h2>
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
                            v-for="rolePermission in permissions"
                            :key="rolePermission.id"
                            class="border-b"
                        >
                            <TableData> {{ rolePermission.id }}</TableData>
                            <TableData> {{ rolePermission.name }}</TableData>
                            <TableData>
                                <Link
                                    :href="
                                        route(
                                            'permissions.destroy',
                                            rolePermission.id
                                        )
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
                                            d="M9.75 9.75l4.5 4.5m0-4.5l-4.5 4.5M21 12a9 9 0 11-18 0 9 9 0 0118 0z"
                                        />
                                    </svg>

                                    <span class="sr-only"
                                        >Icon description</span
                                    >
                                </Link>
                            </TableData>
                        </TableRow>
                    </template>
                </Table>
            </div>
        </div>
    </AdminLayout>
</template>
<style src="vue-multiselect/dist/vue-multiselect.css"></style>
