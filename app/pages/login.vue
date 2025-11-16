<template>
    <div class="h-dvh pt-12 pb-16 flex flex-col gap-8 items-center justify-between ">
        <div class="icon">
            <img src="/icon/app-icon.svg" alt="">
        </div>
        <div class="min-w-64 bg-sky-100 rounded-xl p-4 text-gray-800">
            <section v-if="step == 1">
                <h1 class="text-2xl">Enter your mobile number / Email</h1>
                <!-- <p>Ger your groceries in as fast as one hour</p> -->
                <div class="form flex flex-col my-4">
                    <label class="text-sm">Mobile Number / Email</label>
                    <input type="text" v-model="mobile" class="field">
                    <small v-show="error" class="text-rose-600 mt-4">{{error}}</small>
                </div>
            </section>
            <section v-if="step == 2">
                <h1 class="text-2xl">Enter your 4-digit code</h1>
                <!-- <p>Ger your groceries in as fast as one hour</p> -->
                <div class="form flex flex-col my-4">
                    <label class="text-sm">Code</label>
                    <input type="text" v-model="otp" class="field">
                    <small v-show="error" class="text-rose-600 mt-4">{{error}}</small>
                </div>
                <p class="mt-8 mb-4" >Did not receive the code <button type="button" class="btn-link">Resend</button></p>
            </section>
        </div>
        <div class="min-w-64 flex justify-between ">
            <button type="button" class="btn-back" @click="backAction"><img src="/icon/back.svg" alt=""></button>
            <button type="button" class="btn-primary" @click="submitForm" >Next</button>
        </div>
    </div>
</template>
<script setup>
import { ref } from "vue";
import { useRouter } from "vue-router"
import { navigateTo } from '#app'
const router = useRouter()
const mobile = ref();
const otp = ref()
const error = ref(false)

const step = ref(1)

const submitForm = () => {
    // console.log(mobile.value)
    error.value = false
    if (step.value == 1) {
        if (mobile.value) {
            error.value = false
            step.value += 1
        } else {
            error.value = "Empty field"
        }
    }
    if (step.value == 2) {
        if (otp.value) {
            error.value = false
            // step.value += 1
            navigateTo("/location")
        } else {
            error.value = "Empty field"
        }
    }
}
const backAction = () => {
    if (step.value > 1) {
        step.value -= 1
    } else {
        router.back()
    }
}
</script>
<style lang="css" scoped>
</style>