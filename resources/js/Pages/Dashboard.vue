<template>
    <app-layout title="Dashboard">
        <template #header>
            <h2 class="font-semibold text-xl text-gray-800 leading-tight">
                Products
            </h2>
        </template>

        <div class="py-12">
            <div class="max-w-xl mx-auto bg-white text-black border rounded shadow-sm">
                <div class="p-5">
                    <div>
                        <jet-label for="name" value="Name" />
                        <jet-input id="name" type="text" class="mt-1 block w-full text-black" required autofocus autocomplete="name" />
                    </div>
                    <div class="mt-4">
                        <jet-label for="description" value="Description" />
                        <jet-input id="description" type="text" class="mt-1 block w-full text-black" required autofocus autocomplete="description" />
                    </div>
                    <div class="mt-4">
                        <jet-label for="price" value="Price" />
                        <jet-input id="price" type="text" class="mt-1 block w-full text-black" required autofocus autocomplete="price" />
                    </div>
                    <div class="flex items-center justify-end mt-4">
                        <jet-button class="ml-4">
                            Submit
                        </jet-button>
                    </div>
                </div>
            </div>
            <div class="max-w-xl mx-auto bg-white text-black border rounded shadow-sm mt-4">
                <table class="w-full">
                    <thead>
                        <tr>
                            <th class="p-2 border-b">#</th>
                            <th class="p-2 border-b">Title</th>
                            <th class="p-2 border-b">Action</th>
                        </tr>
                    </thead>
                    <tr>
                        <td class="p-2">1</td>
                        <td class="p-2">Action Figure</td>
                        <td class="p-2"><span class="text-red-400">Delete</span></td>
                    </tr>
                </table>
            </div>
        </div>
    </app-layout>
</template>

<script>
    import { defineComponent } from 'vue'
    import AppLayout from '@/Layouts/AppLayout.vue'
    import Welcome from '@/Jetstream/Welcome.vue'
    import JetInput from '@/Jetstream/Input.vue'
    import JetLabel from '@/Jetstream/Label.vue'
    import JetButton from '@/Jetstream/Button.vue'

    export default defineComponent({
        components: {
            AppLayout,
            Welcome,
            JetInput,
            JetLabel,
            JetButton,
        },
    })
</script>
