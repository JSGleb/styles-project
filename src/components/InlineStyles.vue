<template>
    <div v-bind:style="customStyles">Inline styles!</div>
</template>



<script>
export default {
    computed: {
        customStyles() {
            return {
                backgroundColor: 'purple',
                color: 'yellow',
                fontSize: '30px',
                fontStyle: 'italic',
                padding: '15px'
            }
        }
    }
}
</script>