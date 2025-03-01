<template>
    <Head title="Dashboard"/>

    <AuthenticatedLayout>
        <template #header>
            <h2 class="font-semibold text-xl text-gray-800 leading-tight">Dashboard</h2>
        </template>


        <header class="absolute inset-x-0 top-0 z-50 flex h-16 border-b border-gray-900/10">
            <div class="mx-auto flex w-full max-w-7xl items-center justify-between px-4 sm:px-6 lg:px-8">
                <div class="flex flex-1 items-center gap-x-6">
                    <button type="button" class="-m-3 p-3 md:hidden">
                        <span class="sr-only">Open main menu</span>
                        <svg class="size-5 text-gray-900" viewBox="0 0 20 20" fill="currentColor" aria-hidden="true" data-slot="icon">
                            <path fill-rule="evenodd" d="M2 4.75A.75.75 0 0 1 2.75 4h14.5a.75.75 0 0 1 0 1.5H2.75A.75.75 0 0 1 2 4.75ZM2 10a.75.75 0 0 1 .75-.75h14.5a.75.75 0 0 1 0 1.5H2.75A.75.75 0 0 1 2 10Zm0 5.25a.75.75 0 0 1 .75-.75h14.5a.75.75 0 0 1 0 1.5H2.75a.75.75 0 0 1-.75-.75Z" clip-rule="evenodd"/>
                        </svg>
                    </button>
                    <img class="h-8 w-auto" src="https://tailwindui.com/plus-assets/img/logos/mark.svg?color=indigo&shade=600" alt="Your Company">
                </div>
                <nav class="hidden md:flex md:gap-x-11 md:text-sm/6 md:font-semibold md:text-gray-700">
                    <a href="#">Home</a>
                    <a href="#">Invoices</a>
                    <a href="#">Clients</a>
                    <a href="#">Expenses</a>
                </nav>
                <div class="flex flex-1 items-center justify-end gap-x-8">
                    <button type="button" class="-m-2.5 p-2.5 text-gray-400 hover:text-gray-500">
                        <span class="sr-only">View notifications</span>
                        <svg class="size-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true" data-slot="icon">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M14.857 17.082a23.848 23.848 0 0 0 5.454-1.31A8.967 8.967 0 0 1 18 9.75V9A6 6 0 0 0 6 9v.75a8.967 8.967 0 0 1-2.312 6.022c1.733.64 3.56 1.085 5.455 1.31m5.714 0a24.255 24.255 0 0 1-5.714 0m5.714 0a3 3 0 1 1-5.714 0"/>
                        </svg>
                    </button>
                    <a href="#" class="-m-1.5 p-1.5">
                        <span class="sr-only">Your profile</span>
                        <img class="size-8 rounded-full bg-gray-800" src="https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="">
                    </a>
                </div>
            </div>
            <!-- Mobile menu, show/hide based on menu open state. -->
            <div class="lg:hidden" role="dialog" aria-modal="true">
                <!-- Background backdrop, show/hide based on slide-over state. -->
                <div class="fixed inset-0 z-50"></div>
                <div class="fixed inset-y-0 left-0 z-50 w-full overflow-y-auto bg-white px-4 pb-6 sm:max-w-sm sm:px-6 sm:ring-1 sm:ring-gray-900/10">
                    <div class="-ml-0.5 flex h-16 items-center gap-x-6">
                        <button type="button" class="-m-2.5 p-2.5 text-gray-700">
                            <span class="sr-only">Close menu</span>
                            <svg class="size-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true" data-slot="icon">
                                <path stroke-linecap="round" stroke-linejoin="round" d="M6 18 18 6M6 6l12 12"/>
                            </svg>
                        </button>
                        <div class="-ml-0.5">
                            <a href="#" class="-m-1.5 block p-1.5">
                                <span class="sr-only">Your Company</span>
                                <img class="h-8 w-auto" src="https://tailwindui.com/plus-assets/img/logos/mark.svg?color=indigo&shade=600" alt="">
                            </a>
                        </div>
                    </div>
                    <div class="mt-2 space-y-2">
                        <a href="#" class="-mx-3 block rounded-lg px-3 py-2 text-base/7 font-semibold text-gray-900 hover:bg-gray-50">Home</a>
                        <a href="#" class="-mx-3 block rounded-lg px-3 py-2 text-base/7 font-semibold text-gray-900 hover:bg-gray-50">Invoices</a>
                        <a href="#" class="-mx-3 block rounded-lg px-3 py-2 text-base/7 font-semibold text-gray-900 hover:bg-gray-50">Clients</a>
                        <a href="#" class="-mx-3 block rounded-lg px-3 py-2 text-base/7 font-semibold text-gray-900 hover:bg-gray-50">Expenses</a>
                    </div>
                </div>
            </div>
        </header>

        <main>
            <div class="relative isolate overflow-hidden pt-16">
                <!-- Secondary navigation -->
                <header class="pb-4 pt-6 sm:pb-6">
                    <div class="mx-auto flex max-w-7xl flex-wrap items-center gap-6 px-4 sm:flex-nowrap sm:px-6 lg:px-8">
                        <h1 class="text-base/7 font-semibold text-gray-900">Cashflow</h1>
                        <div class="order-last flex w-full gap-x-8 text-sm/6 font-semibold sm:order-none sm:w-auto sm:border-l sm:border-gray-200 sm:pl-6 sm:text-sm/7">
                            <a href="#" class="text-indigo-600">Last 7 days</a>
                            <a href="#" class="text-gray-700">Last 30 days</a>
                            <a href="#" class="text-gray-700">All-time</a>
                        </div>
                        <a href="#" class="ml-auto flex items-center gap-x-1 rounded-md bg-indigo-600 px-3 py-2 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">
                            <svg class="-ml-1.5 size-5" viewBox="0 0 20 20" fill="currentColor" aria-hidden="true" data-slot="icon">
                                <path d="M10.75 6.75a.75.75 0 0 0-1.5 0v2.5h-2.5a.75.75 0 0 0 0 1.5h2.5v2.5a.75.75 0 0 0 1.5 0v-2.5h2.5a.75.75 0 0 0 0-1.5h-2.5v-2.5Z"/>
                            </svg>
                            New invoice
                        </a>
                    </div>
                </header>

                <!-- Stats -->
                <div class="border-b border-b-gray-900/10 lg:border-t lg:border-t-gray-900/5">
                    <dl class="mx-auto grid max-w-7xl grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 lg:px-2 xl:px-0">
                        <div class="flex flex-wrap items-baseline justify-between gap-x-4 gap-y-2 border-t border-gray-900/5 px-4 py-10 sm:px-6 lg:border-t-0 xl:px-8">
                            <dt class="text-sm/6 font-medium text-gray-500">Revenue</dt>
                            <dd class="text-xs font-medium text-gray-700">+4.75%</dd>
                            <dd class="w-full flex-none text-3xl/10 font-medium tracking-tight text-gray-900">$405,091.00</dd>
                        </div>
                        <div class="flex flex-wrap items-baseline justify-between gap-x-4 gap-y-2 border-t border-gray-900/5 px-4 py-10 sm:border-l sm:px-6 lg:border-t-0 xl:px-8">
                            <dt class="text-sm/6 font-medium text-gray-500">Overdue invoices</dt>
                            <dd class="text-xs font-medium text-rose-600">+54.02%</dd>
                            <dd class="w-full flex-none text-3xl/10 font-medium tracking-tight text-gray-900">$12,787.00</dd>
                        </div>
                        <div class="flex flex-wrap items-baseline justify-between gap-x-4 gap-y-2 border-t border-gray-900/5 px-4 py-10 sm:px-6 lg:border-l lg:border-t-0 xl:px-8">
                            <dt class="text-sm/6 font-medium text-gray-500">Outstanding invoices</dt>
                            <dd class="text-xs font-medium text-gray-700">-1.39%</dd>
                            <dd class="w-full flex-none text-3xl/10 font-medium tracking-tight text-gray-900">$245,988.00</dd>
                        </div>
                        <div class="flex flex-wrap items-baseline justify-between gap-x-4 gap-y-2 border-t border-gray-900/5 px-4 py-10 sm:border-l sm:px-6 lg:border-t-0 xl:px-8">
                            <dt class="text-sm/6 font-medium text-gray-500">Expenses</dt>
                            <dd class="text-xs font-medium text-rose-600">+10.18%</dd>
                            <dd class="w-full flex-none text-3xl/10 font-medium tracking-tight text-gray-900">$30,156.00</dd>
                        </div>
                    </dl>
                </div>

                <div class="absolute left-0 top-full -z-10 mt-96 origin-top-left translate-y-40 -rotate-90 transform-gpu opacity-20 blur-3xl sm:left-1/2 sm:-ml-96 sm:-mt-10 sm:translate-y-0 sm:rotate-0 sm:transform-gpu sm:opacity-50" aria-hidden="true">
                    <div class="aspect-[1154/678] w-[72.125rem] bg-gradient-to-br from-[#FF80B5] to-[#9089FC]" style="clip-path: polygon(100% 38.5%, 82.6% 100%, 60.2% 37.7%, 52.4% 32.1%, 47.5% 41.8%, 45.2% 65.6%, 27.5% 23.4%, 0.1% 35.3%, 17.9% 0%, 27.7% 23.4%, 76.2% 2.5%, 74.2% 56%, 100% 38.5%)"></div>
                </div>
            </div>
        </main>


        <div class="mx-auto bg-white">
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
