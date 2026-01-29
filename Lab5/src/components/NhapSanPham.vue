<script setup>
import { ref } from 'vue';

const emit = defineEmits(['add-product']);

const newProduct = ref({
    name: '',
    description: '',
    price: 0
});

const submitProduct = () => {
    emit('add-product', { ...newProduct.value });

    newProduct.value = {
        name: '',
        description: '',
        price: 0
    };
};
</script>

<template>
    <div class="container mt-3">
        <div class="card p-4 shadow-sm">
            <h3 class="text-center mb-3">Thêm sản phẩm mới</h3>
            <form @submit.prevent="submitProduct">
                <div class="mb-3">
                    <label class="form-label">Tên sản phẩm</label>
                    <input v-model="newProduct.name" type="text" class="form-control" placeholder="Nhập tên sản phẩm" required>
                </div>
                <div class="mb-3">
                    <label class="form-label">Mô tả</label>
                    <input v-model="newProduct.description" type="text" class="form-control" placeholder="Nhập mô tả" required>
                </div>
                <div class="mb-3">
                    <label class="form-label">Giá tiền</label>
                    <input v-model="newProduct.price" type="number" class="form-control" placeholder="Nhập giá" required>
                </div>
                <button type="submit" class="btn btn-success w-100">Thêm sản phẩm</button>
            </form>
        </div>
    </div>
</template>