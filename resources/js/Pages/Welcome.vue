<template>
    <Head title="Home" />

    <home-layout>
        <h1 class="text-lg mb-4 font-bold">Latest Product</h1>
        <div class="grid grid-cols-3 gap-4" >
            <div class="card bordered">
                <figure>
                    <img src="https://picsum.photos/id/1005/400/250">
                </figure> 
                <div class="card-body">
                    <Link class="card-title text-accent">Action Figure</Link>
                    <div class="flex justify-between">
                        <h2 class="text-lg font-medium">Rp10000</h2>
                        <button class="btn btn-primary btn-sm">Buy Now</button>
                    </div>
                </div>
            </div> 
        </div>
    </home-layout>
</template>

<script>
    import { defineComponent } from 'vue'
    import HomeLayout from '@/Layouts/HomeLayout.vue'
    import { Head, Link } from '@inertiajs/inertia-vue3';

    export default defineComponent({
        components: {
            Head,
            Link,
            HomeLayout,
        },
    })
</script>
