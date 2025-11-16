<template>
    <!-- <header class="bg-white p-2">
        <div class="flex items-center justify-center gap-1 my-2 text-xl"><img src="/icon/map-pointer.svg" alt=""> Your current location</div>
        <div class="flex items-center gap-2">
            <input type="search" class="bg-slate-100 p-2 w-full rounded-xl" placeholder="Search" name="" id="">
            <button class="text-sky-400 border border-sky-400 rounded-lg p-1 cursor-pointer">
                <ShoppingCart :size="28" :stroke-width="1" />
            </button>
        </div>
    </header> -->
    <div class="offers m-2">
        <figure>
            <img src="/img/banner.jpg" class="w-full rounded-lg" alt="">
        </figure>
    </div>
    <!-- offers -->
    <div class="offer-carousel p-2">
        <div class="heading flex items-center justify-between my-2">
            <h3 class="font-bold text-2xl">Exclusive Offer</h3>
            <small class="text-gray-500">from stores near you</small>
            <nuxt-link to="/offers" class="text-lg underline text-sky-600">See all</nuxt-link>
        </div>
        <div class="flex gap-2 overflow-auto">
            <div class="card bg-white ">
                <figure>
                    <img src="/img/cdd49d63a82af5cf4cfd7f408c9a57cd24bf47c9.png" alt="">
                </figure>
                <div class="title">Organic Bananas</div>
                <p>6pcs, Priceg</p>
                <div class="flex justify-between mt-1 p-2">
                    <div class="price">39</div>
                    <button class="text-green-500"><CirclePlus :size="32" :stroke-width="1" /></button>
                </div>
            </div>
            <div class="card bg-gradient-to-b from-white to-yellow-50">
                <figure>
                    <img src="/img/accb1df0583c96a67f2ad989598f353de49e5a14.png" alt="">
                </figure>
                <div class="title">Red Apple</div>
                <p>1kg, Priceg</p>
                <div class="flex justify-between mt-1 p-2">
                    <div class="price">249</div>
                    <button class="btn-back"><Plus :size="28" :stroke-width="2" /></button>
                </div>
            </div>
            <div class="card bg-gradient-to-b from-white from-40% via-yellow-100 via-60% to-yellow-50">
                <figure>
                    <img src="/img/3834f4b9c7c2628935f610ab8527d0b21e102632.png" alt="">
                </figure>
                <div class="title">Ginger</div>
                <p>250g, Priceg</p>
                <div class="flex justify-between mt-1 p-2">
                    <div class="price">49</div>
                    <button class="text-green-500"><DiamondPlus :size="32" :stroke-width="1" /></button>
                </div>
            </div>
            <div class="card bg-gradient-to-b from-white to-yellow-100">
                <figure>
                    <img src="/img/3834f4b9c7c2628935f610ab8527d0b21e102632.png" alt="">
                </figure>
                <div class="title">Ginger</div>
                <p>250g, Priceg</p>
                <div class="flex justify-between mt-1 p-2">
                    <div class="price">49</div>
                    <button class="text-green-500"><DiamondPlus :size="32" :stroke-width="1" /></button>
                </div>
            </div>
        </div>
    </div>
    <!-- best selling -->
    <div class="offer-carousel p-2">
        <div class="heading flex items-center justify-between my-2">
            <h3 class="font-semibold text-2xl">Best selling</h3>
            <nuxt-link to="/offers" class="underline text-sky-600">See all</nuxt-link>
        </div>
        <div class="flex gap-2 overflow-auto">
            <div class="card bg-white ">
                <figure>
                    <img src="/img/0c425b7d8f0836dfb36395e62d0c84d6b0af4cf0.png" alt="">
                </figure>
                <div class="title">Organic Bananas</div>
                <p>6pcs, Priceg</p>
                <div class="flex justify-between mt-1 p-2">
                    <div class="price">39</div>
                    <div class="flex items-center border border-green-500 rounded-full">
                        <button class="text-green-500"><CircleMinus :size="32" :stroke-width="1" /></button>
                        <output class="px-1">2</output>
                        <button class="text-green-500"><CirclePlus :size="32" :stroke-width="1" /></button>
                    </div>
                    <!-- <button class="btn-back"><img src="/icon/plus-white.svg" alt=""></button> -->
                </div>
            </div>
            <div class="card bg-gradient-to-b from-white to-slate-100">
                <figure>
                    <img src="/img/accb1df0583c96a67f2ad989598f353de49e5a14.png" alt="">
                </figure>
                <div class="title">Red Apple</div>
                <p>1kg, Priceg</p>
                <div class="flex justify-between mt-1 p-2">
                    <div class="price">249</div>
                    <button class="text-green-500"><DiamondPlus :size="32" :stroke-width="1" /></button>
                    <!-- <button class="btn-back"><img src="/icon/plus-white.svg" alt=""></button> -->
                </div>
            </div>
            <div class="card bg-gradient-to-b from-white from-40% via-slate-200 via-60% to-slate-50">
                <figure>
                    <img src="/img/10f6d5b484482669b38064b6039c1e9dd1e416f7.png" alt="">
                </figure>
                <div class="title">Ginger</div>
                <p>250g, Priceg</p>
                <div class="flex justify-between mt-1 p-2">
                    <div class="price">49</div>
                    <button class="btn-back"><Plus :size="28" :stroke-width="2" /></button>
                </div>
            </div>
            <div class="card bg-gradient-to-b from-white to-slate-200">
                <figure>
                    <img src="/img/10f6d5b484482669b38064b6039c1e9dd1e416f7.png" alt="">
                </figure>
                <div class="title">Ginger</div>
                <p>250g, Priceg</p>
                <div class="flex justify-between mt-1 p-2">
                    <div class="price">49</div>
                    <button class="btn-back"><Plus :size="28" :stroke-width="2" /></button>
                </div>
            </div>
        </div>
    </div>
    <!-- order again -->
    <div class="offer-carousel p-2">
        <div class="heading flex items-center justify-between my-2">
            <h3 class="font-semibold text-xl">Order again</h3>
            <nuxt-link to="/offers" class="underline text-sky-600">See all</nuxt-link>
        </div>
        <div class="flex gap-2 overflow-auto">
            <div class="card bg-white ">
                <figure>
                    <img src="/img/e2faac00a6029bf4a611c1016eaf4b8f75db6d65.png" alt="">
                </figure>
                <!-- <div class="title">Organic Bananas</div> -->
                <p>11 items</p>
                <div class="flex border-t border-slate-200 mt-1 p-2">
                    <button class="btn-secondary">Grocery</button>
                </div>
            </div>
            <div class="card bg-gradient-to-b from-white to-stone-200">
                <figure>
                    <img src="/img/ca51c56fc6c319bfab3990da934ed0eb9c5ae3e7.png" alt="">
                </figure>
                <!-- <div class="title">Red Apple</div> -->
                <p>7 items</p>
                <div class="flex border-t border-stone-300 mt-1 p-2">
                    <button class="btn-secondary">Fruits</button>
                </div>
            </div>
            <div class="card bg-gradient-to-b from-white from-30% via-stone-200 via-50% to-stone-50 to-80%">
                <figure>
                    <img src="/img/cf75912987c6a2d11af9c6213699a2c5c6e3fb48.png" alt="">
                </figure>
                <!-- <div class="title">Ginger</div> -->
                <p>4 items</p>
                <div class="flex border-t border-stone-300 mt-1 p-2">
                    <button class="btn-secondary">Drinks</button>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
import { ref } from "vue"
import { ShoppingCart, CirclePlus, CircleMinus, Plus, DiamondPlus, DiamondMinus  } from 'lucide-vue-next';
definePageMeta({
  layout: 'user',
})
</script>
<style lang="css" scoped>
header {
    input {}
}
</style>