<template>
    <div>
        <!-- <pre>default layout</pre> -->
        <slot />
    </div>
</template>
<script>
export default {

    name: 'default',

    data() {
        return {

        }
    }
}
</script>
<style lang="css" scoped>
div {
    background-color: lightgreen;
    background-image: url('./img/intro.jpg');
    background-repeat: no-repeat;
    background-position: center top;
    background-size: cover;
}
</style>