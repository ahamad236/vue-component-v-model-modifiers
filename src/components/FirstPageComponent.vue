<!-- <template>
    <h2>
        First Page Component
    </h2>
    <div>
        userName in Child : {{ model }}
    </div>
    <input v-model="model"/>
</template>

<script setup lang="ts">
    const [model, modifiers] = defineModel({
        set(value:string){
            if(modifiers.capitalize){
                return value.charAt(0).toUpperCase()+value.slice(1)
            }
            return value
        }
    })
</script> -->



<!-- v-model modifiers with arguments starts from here -->
<template>
    <h2> First Page Component </h2>
    <input v-model="firstName"/>
    <input v-model="lastName"/>
</template>
<script setup lang="ts">
    const [firstName, firstNameModifiers] = defineModel('firstName')
    const [lastName, lastNameModifiers] = defineModel('lastName')

    console.log(firstNameModifiers.capitalize)
    console.log(lastNameModifiers.upperCase)
</script>
<!-- v-model modifiers upto above -->