<script setup></script>

<template>
    <div class="relative overflow-x-auto shadow-md sm:rounded-lg">
        <table class="min-w-full text-center text-sm font-light">
            <thead
                class="text-xs text-gray-700 uppercase bg-gray-50 dark:bg-gray-700 dark:text-gray-400"
            >
                <slot name="header"></slot>
            </thead>
            <tbody>
                <slot></slot>
            </tbody>
        </table>
    </div>
</template>
