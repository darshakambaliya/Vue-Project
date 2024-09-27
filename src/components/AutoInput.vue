<template>
    <span class="material-icons">search</span>
    <input class="border-none" :placeholder="placeholder"/>
</template>

<script>
export default {
  name: "AutoInput",
props: {
    placeholder: '',
}

};
</script>

<style scoped>
/* Add any specific styles if needed */
</style>