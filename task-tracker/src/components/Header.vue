<template>
    <header>
        <h1>{{title}}</h1>
        <ButtonComponent/>
    </header>
</template>

<script>
import ButtonComponent from './Button.vue'
// import { defineComponent } from '@vue/composition-api'

// export default defineComponent({
//     setup() {
//     },
// })

export default {
    name: 'HeaderComponent',
    // props: ['title'],
    // props: {
    //     title: {
    //         type: String,
    //         default: 'Hello World'
    //     }
    // },
    components: {
        ButtonComponent
    },
    props: {
        title: String
    },

    data () {
    }
}

</script>

<style scoped>
    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 20px;
    }
</style>
