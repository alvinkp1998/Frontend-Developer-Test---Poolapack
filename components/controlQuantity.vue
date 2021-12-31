<template>
  <div>
    <button class="btn btn-decrease" @click="kurang">
      <i class="fas fa-minus"></i>
    </button>
    <span class="quantity text-center"> {{ jumlah }} </span>
    <button class="btn btn-increase" @click="tambah">
      <i class="fas fa-plus"></i>
    </button>
  </div>
</template>

<script>
export default {
  props: {
    jumlah: Number,
  },
  methods: {
    tambah() {
      this.$emit("tambah", this.jumlah);
    },
    kurang() {
      this.$emit("kurang", this.jumlah);
    },
  },
};
</script>
<style scoped>
.btn-decrease {
  color: gray;
  border: 2px solid gray;
}
.btn-increase {
  color: #f9be00;
  border: 2px solid #f9be00;
}

.quantity {
  padding: 5px 15px 5px 15px;
}
</style>
