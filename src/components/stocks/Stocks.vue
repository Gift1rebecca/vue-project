<template>
    <div>
        <app-stock v-for="stock in stocks"</app-stock>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                stocks: [
                    { id: 1, name: 'BMW', price: 110 },
                    { id: 2, name: 'Goggle', price: 200 },
                    { id: 3, name: 'Apple', price: 250 },
                    { id: 4, name: 'Twitter', price: 8 },
                ]
            }
        },
        components: {
            appStock: Stock
        }
    }
</script>