<template>
    <div>
        <sliders/>
        <products/>
        <contact/>
    </div>
</template>
<script>
import sliders from './sliders.vue'
import contact from './contact.vue'
import products from './products/products.vue'

export default {
    name : 'home',
    components: {
        sliders,products,contact
    }
}
</script>