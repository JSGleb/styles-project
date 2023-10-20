<template>
    <!-- <div :class="{'active': isActive, 'disabled': isDisabled}">Class Styles!</div> -->

    <div>
        <button @click="switchBtn">Switcher</button>
        <button :class="btnClass">{{ btnText }}</button>
    </div>
</template>

<script>
export default {
    data() {
        return {
            isActive: true,
            isDisabled: false,
            btnText: 'Click on me!'
        }
    },

    methods: {
        switchBtn() {
            this.isActive = !this.isActive;
            this.isDisabled = !this.isDisabled;
        }
    },

    computed: {
        btnClass() {
            return {
                'active': this.isActive,
                'disabled': this.isDisabled
            }
        }
    }
}
</script>

<style scoped>
    button:nth-of-type(2) {
        font-size: 2em;
        width: 100%;
        padding: 20px;
    }
    .active {
        background-color: darkgreen;
        color: whitesmoke;
        cursor: pointer;
        transition: all .4s ease-in;
    }
    .active:hover {
        background-color: red;
    }

    .disabled {
        opacity: .5;
        cursor: not-allowed;
        padding: 20px;
    }

</style>