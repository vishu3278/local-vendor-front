<template>
    <div class="max-w-6xl mx-auto " >
        <NuxtRouteAnnouncer>
            <template #default="{ message }">
                <p>{{ message }} was loaded.</p>
            </template>
        </NuxtRouteAnnouncer>
        <!-- <NuxtWelcome /> -->
        <NuxtLayout>
            <NuxtPage />
        </NuxtLayout>
    </div>
</template>
<style>
.page-enter-active,
.page-leave-active {
    transition: all 0.4s;
}

.page-enter-from,
.page-leave-to {
    opacity: 0;
    filter: blur(1rem);
}

.layout-enter-active,
.layout-leave-active {
    transition: all 0.35s;
}
.layout-enter-from,
.layout-leave-to {
    opacity: 0;
    filter: grayscale(1);
}
</style>