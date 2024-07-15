<template>
    <div class="phone-number">
        <p>{{label}}</p>
        <a href="tel:0800-PHONE-ME" v-for="phone in phoneNumbers" :key="phone"> <span class="material-icons">phone</span> {{ phone }}</a>
    </div>
</template>

<script>
export default {
    props: {
        label: {
            type: Number,
            required: false
        },
        phoneNumbers: {
            type: Array,
            required: false
        }
    }
}
</script>