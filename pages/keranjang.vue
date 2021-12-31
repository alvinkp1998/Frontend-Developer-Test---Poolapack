<template>
  <div>
    <div class="row mb-5">
      <div class="col-md-9">
        <div class="card shadow-sm">
          <div class="card-body">
            <div class="card-title">
              <h3>
                <strong> Keranjang</strong>
              </h3>
              <hr />
              <div class="card-text" style="padding-left: 12px">
                <input
                  type="checkbox"
                  aria-label="Checkbox for following text input"
                />
                <span>Pilih Semua Pesanan (0)</span>
              </div>
            </div>
          </div>
        </div>
        <div class="card shadow-sm mt-5" style="border-radius: 20px">
          <div class="card-body" style="padding-bottom: 0px !important">
            <div class="float-left mr-2 mt-2">
              <input
                type="checkbox"
                aria-label="Checkbox for following text input"
              />
            </div>
            <div style="height: 80px" class="float-left">
              <img
                src="assets/img/pp-seller.png"
                alt="pp seller"
                class="mr-2"
              />
            </div>

            <p style="margin-bottom: 0px !important">
              <strong
                >Bahtera Bara
                <img src="assets/img/check.png" class="mb-1 ml-3" /><span
                  style="color: #176ef0; margin-left: -4px"
                  >erified</span
                >
              </strong>
              <br />
              <span class="gray">Kab. Bandung </span>
            </p>
          </div>
          <hr class="m-0" />
          <div class="card-body">
            <div class="float-left mr-2" style="height: 150px">
              <input
                type="checkbox"
                aria-label="Checkbox for following text input"
              />
              <span
                ><img
                  src="assets/img/produk.jpg"
                  width="80px"
                  height="80px"
                  class="ml-3"
              /></span>
            </div>
            <div class="produk">
              <span>
                <h6><strong> Poly PE MVS L158 100 / 70</strong></h6>

                <p>
                  MOQ: 100 Meter <br />
                  <span class="font-smaller">Kelipatan Order: 100 Meter</span>
                </p>
              </span>

              <select
                class="custom-select mr-4"
                id="inputGroupSelect01"
                style="width: 300px"
              >
                <option selected>Varian: Lorem Ipsum</option>
                <option value="1">Varian: Lorem Ipsum 2</option>
                <option value="2">Varian: Lorem Ipsum 3</option>
                <option value="3">Varian: Lorem Ipsum 4</option>
              </select>
              <span> <strong> Rp.00.0000/Meter</strong> </span>
              <span class="ml-4 mr-4"
                ><button class="btn btn-quantity">
                  <i class="fas fa-minus"></i>
                </button>
                <span class="ml-2 mr-2 pr-1">0</span
                ><button class="btn btn-quantity">
                  <i class="fas fa-plus"></i></button
              ></span>
              <span>
                <strong>Rp.00.0000</strong>
                <i
                  class="far fa-trash-alt ml-5"
                  style="color: red; cursor: pointer"
                ></i>
              </span>
            </div>
            <hr />
          </div>
        </div>
      </div>
      <div class="col-md-3">
        <div class="card shadow-sm">
          <div class="card-body">
            <div class="card-title">
              <h5><strong>Ringkasan</strong></h5>
            </div>
            <div class="card-text pt-2">
              <p class="float-left">Total Harga:</p>
              <p class="float-right">Rp.00.0000</p>
            </div>
            <div style="clear: both">
              <p class="float-left">Diskon:</p>
              <p class="float-right">Rp.0</p>
            </div>
            <div style="clear: both"></div>
            <hr />
            <p class="float-left"><span class="gray">Total Harga</span></p>
            <p class="float-right"><strong>Rp.00.000</strong></p>
            <button class="btn btn-main btn-block">
              <strong> Buat Pesanan (0)</strong>
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  layout: "dashboard",
};
</script>

<style scoped>
.btn-main {
  color: white;
  background-color: #f9be00;
}

.font-smaller {
  font-size: 15px;
}

.btn-quantity {
  background-color: white;
  border: 1px solid black;
}
</style>
