<template>
    <header class="bg-white p-2">
        <div class="flex items-center justify-center gap-1 my-2 text-xl"><img src="/icon/map-pointer.svg" alt=""> Your current location</div>
        <input type="search" class="bg-slate-100 p-2 w-full rounded-xl" placeholder="Search" name="" id="">
    </header>
    <div class="offers m-2">
        <figure>
            <img src="/img/banner.jpg" class="w-full rounded-lg" alt="">
        </figure>
    </div>
    <!-- offers -->
    <div class="offer-carousel p-2">
        <div class="heading flex items-center justify-between my-2">
            <h3 class="font-bold text-2xl">Exclusive Offer</h3>
            <nuxt-link to="/offers" class="text-xl text-sky-600">See all</nuxt-link>
        </div>
        <div class="flex gap-2 overflow-auto">
            <div class="card bg-gradient-to-b from-white to-yellow-100">
                <figure>
                    <img src="/img/cdd49d63a82af5cf4cfd7f408c9a57cd24bf47c9.png" alt="">
                </figure>
                <div class="title">Organic Bananas</div>
                <p>6pcs, Priceg</p>
                <div class="flex justify-between mt-2 p-2">
                    <div class="price">39</div>
                    <button class="btn-back"><img src="/icon/plus-white.svg" alt=""></button>
                </div>
            </div>
            <div class="card bg-gradient-to-b from-white to-yellow-100">
                <figure>
                    <img src="/img/accb1df0583c96a67f2ad989598f353de49e5a14.png" alt="">
                </figure>
                <div class="title">Red Apple</div>
                <p>1kg, Priceg</p>
                <div class="flex justify-between mt-2 p-2">
                    <div class="price">249</div>
                    <button class="btn-back"><img src="/icon/plus-white.svg" alt=""></button>
                </div>
            </div>
            <div class="card bg-gradient-to-b from-white to-yellow-100">
                <figure>
                    <img src="/img/3834f4b9c7c2628935f610ab8527d0b21e102632.png" alt="">
                </figure>
                <div class="title">Ginger</div>
                <p>250g, Priceg</p>
                <div class="flex justify-between mt-2 p-2">
                    <div class="price">49</div>
                    <button class="btn-back"><img src="/icon/plus-white.svg" alt=""></button>
                </div>
            </div>
        </div>
    </div>
    <!-- best selling -->
    <div class="offer-carousel p-2">
        <div class="heading flex items-center justify-between my-2">
            <h3 class="font-bold text-2xl">Best selling</h3>
            <nuxt-link to="/offers" class="text-xl text-sky-600">See all</nuxt-link>
        </div>
        <div class="flex gap-2 overflow-auto">
            <div class="card bg-gradient-to-b from-white to-slate-200">
                <figure>
                    <img src="/img/0c425b7d8f0836dfb36395e62d0c84d6b0af4cf0.png" alt="">
                </figure>
                <div class="title">Organic Bananas</div>
                <p>6pcs, Priceg</p>
                <div class="flex justify-between mt-2 p-2">
                    <div class="price">39</div>
                    <button class="btn-back"><img src="/icon/plus-white.svg" alt=""></button>
                </div>
            </div>
            <div class="card bg-gradient-to-b from-white to-slate-200">
                <figure>
                    <img src="/img/accb1df0583c96a67f2ad989598f353de49e5a14.png" alt="">
                </figure>
                <div class="title">Red Apple</div>
                <p>1kg, Priceg</p>
                <div class="flex justify-between mt-2 p-2">
                    <div class="price">249</div>
                    <button class="btn-back"><img src="/icon/plus-white.svg" alt=""></button>
                </div>
            </div>
            <div class="card bg-gradient-to-b from-white to-slate-200">
                <figure>
                    <img src="/img/10f6d5b484482669b38064b6039c1e9dd1e416f7.png" alt="">
                </figure>
                <div class="title">Ginger</div>
                <p>250g, Priceg</p>
                <div class="flex justify-between mt-2 p-2">
                    <div class="price">49</div>
                    <button class="btn-back"><img src="/icon/plus-white.svg" alt=""></button>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
import { ref } from "vue"
</script>
<style lang="css" scoped>
header {
    input {}
}
</style>