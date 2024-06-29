<template>
    <div class="w-full">
        <HeaderBoard />

        <div class="flex justify-between mx-16 p-4">
            <div>
                <h3>All Boards</h3>
            </div>
            <div>
                <n-input :value="value" type="text" placeholder="Filter boards" />
            </div>

        </div>

    </div>
</template>

<script>
import HeaderBoard from '../layout/HeaderBoard.vue';
import { defineComponent, ref } from 'vue';

export default defineComponent({
    name: 'MyComponent',
    components: {
        HeaderBoard,
    },
    setup() {
        const value = ref(null);

        return {
            value,
        };
    },
});
</script>

<style scoped>

</style>
