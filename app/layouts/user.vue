<template>
    <div>
        <header class="bg-white p-2 sticky top-0">
            <div class="flex items-center justify-center gap-1 my-2 text-xl"><img src="/icon/map-pointer.svg" alt=""> Your current location</div>
            <div class="flex items-center gap-2">
                <input type="search" class="bg-slate-100 p-2 w-full rounded-xl" placeholder="Search" name="" id="">
                <button class="text-sky-400 border border-sky-400 rounded-lg p-1 shrink-0 cursor-pointer">
                    <ShoppingCart :size="28" :stroke-width="1" />
                </button>
            </div>
        </header>
        <slot />
    </div>
</template>
<script setup>
import { ShoppingCart } from 'lucide-vue-next';

</script>
<style lang="css" scoped>
div {
    /*background-color: var(--color-sky-200);*/
    /*background-image: url('./img/intro.jpg');
    background-repeat: no-repeat;
    background-position: center top;
    background-size: cover;*/
}
</style>