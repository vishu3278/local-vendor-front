<template>
    <div class="h-dvh pb-16 flex flex-col gap-4 justify-between ">
        <div class="map-wrapper">
            <img src="/img/GoogleMapTA.webp" class="w-full h-full object-cover" alt="">
        </div>
        <div class="min-w-64 bg-sky-100 rounded-xl p-4 mx-4 text-gray-800">
            <section>
                <h1 class="text-2xl">Select Your Location</h1>
                <div class="grid grid-cols-1 md:grid-cols-2 md:gap-2">
                    <div class="form flex flex-col my-4">
                        <label class="text-sm">Add your address</label>
                        <input type="text" v-model="address" class="field">
                        <small v-show="error" class="text-rose-600 mt-4">{{error}}</small>
                    </div>
                    <div class="form flex flex-col my-4">
                        <label class="text-sm">City</label>
                        <input type="text" v-model="city" class="field">
                        <small v-show="error" class="text-rose-600 mt-4">{{error}}</small>
                    </div>
                    <div class="form flex flex-col my-4">
                        <label class="text-sm">State</label>
                        <input type="text" v-model="state" class="field">
                        <small v-show="error" class="text-rose-600 mt-4">{{error}}</small>
                    </div>
                    <div class="form flex flex-col my-4">
                        <label class="text-sm">Pincode</label>
                        <input type="text" v-model="pincode" class="field">
                        <small v-show="error" class="text-rose-600 mt-4">{{error}}</small>
                    </div>
                </div>
            </section>
            <!-- <section v-if="step == 2">
                <h1 class="text-2xl">Enter your 4-digit code</h1>
                <div class="form flex flex-col my-4">
                    <label class="text-sm">Code</label>
                    <input type="text" v-model="otp" class="field">
                </div>
                <p class="mt-8 mb-4">Did not receive the code</p>
                <button type="button" class="btn-secondary">Resend</button>
            </section> -->
        </div>
        <div class="min-w-64 mx-12 flex justify-between ">
            <button type="button" class="btn-back" @click="backAction"><img src="/icon/back.svg" alt=""></button>
            <button type="button" class="btn-primary" @click="submitForm">Next</button>
        </div>
    </div>
</template>
<script setup>
import { ref } from "vue";
import { useRouter } from "vue-router"
import { navigateTo } from '#app'

const router = useRouter()

const location = ref({ latitude: 2.5, longitude: 5.5 });
const address = ref("")
const city = ref("")
const state = ref("")
const pincode = ref("")
const error = ref(false)

const submitForm = () => {
    console.log(address.value)
    navigateTo("/dashboard")
}
const backAction = () => {

}
</script>
<style lang="css" scoped>
.map-wrapper {
    height: 60dvh;
}
</style>