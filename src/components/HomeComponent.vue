<!-- <template>
    <h1>
        Home Component
    </h1>
    <div>userName in Parent : {{userName}}</div>
    <input v-model="userName"/>
    <FirstPage v-model.capitalize="userName"></FirstPage>
</template>

<script setup lang="ts">
    import FirstPage from "./FirstPageComponent.vue"
    import { ref } from 'vue'
    // import type { Ref } from 'vue'

    const userName = ref()
</script> -->



<!-- v-model modifiers with arguments starts from here -->
<template>
    
    <FirstPage v-model.first-name.capitalize="first" v-model.last-name.upperCase="last"></FirstPage>
</template>

<script setup lang="ts">
    import FirstPage from "./FirstPageComponent.vue"
    import { ref } from 'vue'
    
    const first = ref('hai')
    const last = ref('hello')
</script>
<!-- v-model modifiers upto above -->