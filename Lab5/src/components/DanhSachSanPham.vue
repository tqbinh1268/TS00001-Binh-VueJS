<script setup>
defineProps({
  products: {
    type: Array,
    required: true,
  },
});
</script>

<template>
  <div class="container mt-5">
    <h2 class="mb-4 text-center">Danh sách linh kiện máy tính</h2>
    <div class="row row-cols-1 row-cols-md-2 g-4">
      <div class="col" v-for="(product, index) in products" :key="index">
        <div class="card">
          <!-- <img src="..." class="card-img-top" alt="..." /> -->
          <div class="card-body">
            <h5 class="card-title">{{ product.name }}</h5>
            <p class="card-text">
              {{ product.description }}
            </p>
            <h3>{{ product.price}} VNĐ</h3>
          </div>
        </div>
      </div>
      
    </div>
    
    <!-- phần thêm mới -->
    
  </div>
</template>
