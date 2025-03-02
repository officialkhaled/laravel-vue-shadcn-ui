<template>
    <Head title="Dashboard"/>

    <AuthenticatedLayout>
<!--        <template #header>-->
<!--            <h2 class="font-semibold text-xl text-gray-800 leading-tight">Dashboard</h2>-->
<!--        </template>-->

        <div class="mx-auto">
            <div class="max-w-7xl mx-auto grid grid-cols-4 gap-4 p-6">
                <!-- Payment Method -->
                <div class="col-span-1 p-4 bg-white rounded-lg shadow-md">
                    <p class="text-lg font-semibold">Payment Method</p>
                    <div class="mt-4 space-y-2">
                        <div class="flex items-center justify-between bg-gray-100 p-2 rounded-md">
                            <span>Mastercard</span>
                            <span>•••• 2172</span>
                        </div>
                        <div class="flex items-center justify-between bg-gray-100 p-2 rounded-md">
                            <span>VISA</span>
                            <span>•••• 2172</span>
                        </div>
                        <div class="flex items-center justify-between bg-gray-100 p-2 rounded-md">
                            <span>AMEX</span>
                            <span>•••• 2172</span>
                        </div>
                    </div>
                    <button class="mt-4 w-full bg-green-500 text-white p-2 rounded-md shadow-md hover:bg-green-600 focus:ring-1 focus:ring-green-700">
                        Confirm to pay
                    </button>
                </div>

                <!-- Smart Banking -->
                <div class="col-span-1 p-4 bg-white rounded-lg flex items-center shadow-md">
                    <p class="text-2xl font-bold">Smart Banking Smart Living</p>
                </div>

                <!-- User Image -->
                <div class="col-span-1 row-span-2">
                    <img src="https://plus.unsplash.com/premium_photo-1669357657874-34944fa0be68?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
                         alt="User" class="w-full h-full object-cover rounded-lg shadow-md"/>
                </div>

                <!-- Meeting Image -->
                <div class="col-span-1">
                    <img src="https://images.unsplash.com/photo-1570051008600-b34baa49e751?q=80&w=2085&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
                         alt="Meeting" class="w-full h-full object-cover rounded-lg shadow-md"/>
                </div>

                <!-- Total Ads -->
                <div class="col-span-1 p-4 bg-white rounded-lg shadow-md">
                    <div class="flex justify-between">
                        <p class="text-lg font-semibold">Total Ads</p>
                        <div class="text-right">
                            <p class="text-2xl font-bold">725K</p>
                            <p class="text-green-500">+15%</p>
                        </div>
                    </div>
                </div>

                <!-- Stock Intelligence -->
                <div class="col-span-1 p-4 bg-white rounded-lg shadow-md">
                    <div class="flex justify-between">
                        <p class="text-lg font-semibold">Stock Intelligence</p>
                        <p class="text-2xl font-bold">$92,020</p>
                    </div>
                </div>

                <!-- Phone Image -->
                <div class="col-span-1 row-span-2">
                    <img src="https://plus.unsplash.com/premium_photo-1684445034763-013f0525c40c?q=80&w=1974&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
                         alt="Phone" class="w-full h-full object-cover rounded-lg shadow-md"/>
                </div>

                <!-- Organic Position -->
                <div class="col-span-2 p-4 bg-white rounded-lg shadow-md">
                    <div class="flex justify-between">
                        <p class="text-lg font-semibold">Organic Position</p>
                        <p class="text-3xl font-bold">54%</p>
                    </div>
                </div>

                <!-- Trees Image -->
                <div class="col-span-1 rounded-lg shadow-md">
                    <img src="https://images.unsplash.com/photo-1591779051696-1c3fa1469a79?q=80&w=1974&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
                         alt="Phone" class="h-full w-full object-cover rounded-lg shadow-md"/>
                </div>
            </div>
        </div>
    </AuthenticatedLayout>
</template>

<script setup>
import {Head} from '@inertiajs/vue3';
import AuthenticatedLayout from '@/Layouts/AuthenticatedLayout.vue';
</script>
