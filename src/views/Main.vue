<template>
    <div class="app-main">
        <div v-if="windowWidth < 768">
            <Mobile></Mobile>
        </div>
        <div  v-if="windowWidth > 768">
            <Desktop></Desktop>
        </div>
    </div>
</template>

<script>
import Mobile from './Mobile'
import Desktop from './Desktop'

    export default {
        name: "Main",
        components: {
            Mobile,
            Desktop
        },
        data() {
            return {
                windowWidth: window.innerWidth
            }
        }
    }
</script>

<style scoped lang="sass">

</style>
