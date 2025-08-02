<template>
    <div class="container">
    <button @click="goErrorPage">ボタン</button>
    </div>
    </template>

<script setup lang="ts">
import { createError, useRouter, useRoute } from '#app'

const route = useRoute()

const goErrorPage = () => {
throw createError({
    statusCode: 404,
    statusMessage: 'notfound',
    message: 'メッセージ',
    fatal: true,
    data: {
    path: route.fullPath,
    }
    })
}
</script>
