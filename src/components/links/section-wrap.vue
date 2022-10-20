<script setup>
import socialButton from './social-button.vue';
</script>

<template>
<div class="flex w-full justify-center max-w-md border-white mx-auto">
    <social-button link="https://twitter.com/xabi_03" :icon="['fab','twitter']" />
    <social-button link="https://www.linkedin.com/in/xmartinez" :icon="['fab','linkedin']" />
    <social-button link="https://github.com/x4b1" :icon="['fab','github']" />
    <social-button link="https://www.instagram.com/_x4b1_" :icon="['fab','instagram']" />
    <social-button link="mailto:hello@xmartinez.dev" :icon="['far','paper-plane']" />
</div>
</template>
