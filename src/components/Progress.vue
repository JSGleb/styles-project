<template>
    <div>
        <h1>Progress line</h1>
    
        <div class="progress">
            <div :style="progressStyles"></div>
        </div>
    </div>
</template>


<script>
export default {
    name: 'ProgressLine',
    data() {
        return {
            progress: 50
        }
    },
    computed: {
        progressStyles() {
            return {
                width: this.progress + '%',
                backgroundColor: 'blue'
            }
        }
    }
}
</script>

<style>
    .progress {
        width: 100%;
        height: 20px;
        background-color: lightgray;
    }

    .progress > div {
        height: 100%;
    }
</style>