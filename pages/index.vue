<template>
<div class="container">
    <h1>{{ title }}</h1>

    <NuxtLink to="/users/test">usersへ</NuxtLink>

    <p>{{ description }}</p>

    <NuxtLink to="/other">otherへ</NuxtLink>

    <NuxtLogo></NuxtLogo>

    <FooBar message="メッセージ"></FooBar>

</div>
</template>

<script>
import NuxtLogo from '../components/NuxtLogo.vue'

export default {
components: {
NuxtLogo,
},
data() {
return {
title: 'Nuxt.js',
description: 'let`s learn Nuxt.js',
}
},
}

</script>

<style>
.container {
padding: 30px;
}
</style>


<!-- ブランチを切った -->

<!-- feature/test2ブランチ -->
<!-- feature/test2ブランチ2回目 -->
