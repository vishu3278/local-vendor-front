<template>
    <div class="max-w-6xl mx-auto bg-sky-500 " style="background: url(/img/intro.jpg) no-repeat center top / cover;">
        <NuxtRouteAnnouncer>
            <template #default="{ message }">
                <p>{{ message }} was loaded.</p>
            </template>
        </NuxtRouteAnnouncer>
        <!-- <NuxtWelcome /> -->
        <NuxtPage />
    </div>
</template>