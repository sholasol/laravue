<script setup>
import AdminLayout from "@/Layouts/AdminLayout.vue";
import { Head, Link, useForm } from "@inertiajs/vue3";
import PrimaryButton from "@/Components/PrimaryButton.vue";
import InputLabel from "@/Components/InputLabel.vue";
import InputError from "@/Components/InputError.vue";
import TextInput from "@/Components/TextInput.vue";

const props = defineProps({
    permission: {
        type: Object,
        required: true,
    },
});

const form = useForm({
    name: props.permission?.name,
});
</script>

<template>
    <Head title="Edit Permission" />

    <AdminLayout>
        <div class="max-w-7xl mx-auto py-4">
            <div class="flex justify-between">
                <h2 class="font-semibold text-xl text-gray-800 leading-tight">
                    Edit Permission
                </h2>
                <Link
                    :href="route('permissions.index')"
                    class="px-3 py-2 text-white font-semibold bg-indigo-500 hover:bg-indigo-700 rounded"
                >
                    Back
                </Link>
            </div>

            <div class="mt-6 max-w-2xl mx-auto bg-slate-100 shadow-lg p-6">
                <form
                    @submit.prevent="
                        form.put(route('permissions.update', permission.id))
                    "
                >
                    <div>
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

                    <div class="flex items-center mt-4">
                        <PrimaryButton class="ml-4"> Update </PrimaryButton>
                    </div>
                </form>
            </div>
        </div>
    </AdminLayout>
</template>
