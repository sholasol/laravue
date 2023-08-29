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

const props = defineProps({
    user: {
        type: Object,
        required: true,
    },
    roles: Array,
    permissions: Array,
});
const form = useForm({
    name: props.user?.name,
    email: props.user?.email,
    roles: [],
    permissions: [],
});

const submit = () => {
    form.put(route("users.update", props.user.id));
};

// onMounted(() => {
//     form.permissions = props.user?.permissions;
//     form.roles = props.user?.roles;
// });
</script>

<template>
    <Head title="Create User" />

    <AdminLayout>
        <div class="flex justify-between">
            <h2 class="font-semibold text-xl text-gray-800 leading-tight">
                Create User
            </h2>
            <Link
                :href="route('users.index')"
                class="px-3 py-2 text-white font-semibold bg-indigo-500 hover:bg-indigo-700 rounded"
            >
                Back
            </Link>
        </div>

        <div
            class="w-full sm:max-w-6xl mx-auto mt-6 px-6 py-4 bg-white shadow-md overflow-hidden sm:rounded-lg"
        >
            <form @submit.prevent="submit">
                <div class="grid grid-cols-2 gap-4">
                    <!--First name input-->
                    <div class="relative mb-6" data-te-input-wrapper-init>
                        <InputLabel for="name" value="Name" />
                        <TextInput
                            id="name"
                            v-model="form.name"
                            type="text"
                            class="peer block min-h-[auto] w-full rounded border-0 px-3"
                        />

                        <InputError class="mt-2" :message="form.errors.name" />
                    </div>

                    <div class="relative mb-6" data-te-input-wrapper-init>
                        <InputLabel for="email" value="Email" />
                        <TextInput
                            id="email"
                            v-model="form.email"
                            type="email"
                            class="peer block min-h-[auto] w-full rounded border-0 px-3"
                        />

                        <InputError class="mt-2" :message="form.errors.email" />
                    </div>
                    <div class="mb-6">
                        <InputLabel for="permissons" value="Permissions" />
                        <VueMultiselect
                            v-model="form.permissions"
                            :options="permissions"
                            :multiple="true"
                            :close-on-select="true"
                            placeholder="Pick Permissions"
                            label="permissions"
                            track-by="id"
                        />
                    </div>
                    <div class="mb-6">
                        <InputLabel for="roles" value="Roles" />
                        <VueMultiselect
                            v-model="form.roles"
                            :options="roles"
                            :multiple="true"
                            :close-on-select="true"
                            placeholder="Pick Role"
                            label="roles"
                            track-by="id"
                        />
                    </div>
                </div>

                <!--Submit button-->
                <PrimaryButton
                    type="submit"
                    class="inline-block w-full rounded bg-primary px-6 pb-2 pt-2.5 text-xs font-medium uppercase leading-normal text-white"
                    data-te-ripple-init
                    data-te-ripple-color="light"
                >
                    Update User
                </PrimaryButton>
            </form>
        </div>
    </AdminLayout>
</template>
<style src="vue-multiselect/dist/vue-multiselect.css"></style>
