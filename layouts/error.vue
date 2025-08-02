<template>
    <div>
    <div>エラーページです。</div>
    <p>{{ error.statusCode }}</p>
    <p>{{ error.message }}</p>
    <p>{{ error.path }}</p>
    </div>
</template>

<script setup>
    const error = useError()
</script>