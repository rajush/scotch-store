<!-- <template>
<div>
  <div class="title">
    <h1>This is Admin/New</h1>
  </div>
</div>
</template> -->
<template>
  <product-form @save-product="addProduct" :model="model" :manufacturers="manufacturers">
  </product-form>
</template>

<script>
  import ProductFrom from '@/components/products/ProductForm';

  export default {
    data() {
      return {
        model: {},
        manufacturers: [
          {
            _id: 'sam',
            name: 'Samsung',
          },
          {
            _id: 'apple',
            name: 'Apple',
          },
        ],
      };
    },
    methods: {
      addProduct(model) {
        console.log('model', model);
      },
    },
    components: {
      'product-form': ProductFrom,
    },
  };
</script>
