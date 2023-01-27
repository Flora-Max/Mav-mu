<script setup>
 defineProps({
    source: { type: [String, null], required:true, default: null},
  })
</script>

<template>
    <section>
        <div>
            <img src= {{ source }}  alt="">
        </div>
    </section>
</template>