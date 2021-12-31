<template>
  <div>
    <!-- Produk Preview-->
    <div class="row d-flex">
      <div class="col-md-3 mt-2 p-0">
        <img
          src="assets/img/produk.jpg"
          alt="foto produk"
          width="100%"
          class="p-3 foto-produk"
        />
        <div class="d-flex p-3 justify-content-center">
          <img
            src="assets/img/produk.jpg"
            alt="foto produk"
            class="img-list pr-1"
          />

          <img
            src="assets/img/produk.jpg"
            alt="foto produk"
            class="img-list pr-1"
          />
          <img
            src="assets/img/produk.jpg"
            alt="foto produk"
            class="img-list pr-1"
          />
          <img
            src="assets/img/produk.jpg"
            alt="foto produk"
            class="img-list pr-1"
          />

          <img src="assets/img/produk.jpg" alt="foto produk" class="img-list" />
        </div>
      </div>
      <div class="col-md-6" style="padding-left: 3px !important">
        <div class="mt-4">
          <div class="row">
            <div class="col-5">
              <div class="">
                <h4>Poly PE MVS L158 100/70</h4>
                <i class="fa fa-star main-color"></i>
                <i class="fa fa-star main-color"></i>
                <i class="fa fa-star main-color"></i>
                <i class="fa fa-star main-color"></i>
                <i class="fa fa-star main-color"></i>
                <span class="main-color"> <strong>5</strong> </span>
                <span class="border-left pl-1">100</span>
                <span class="gray">Ulasan</span>
                <span class="border-left pl-1"
                  >100 <span class="gray">Terjual</span></span
                >
              </div>
            </div>
            <div class="col-2"></div>
            <div class="col-5">
              <div class="">
                <h4>Berakhir dalam</h4>
                <span class="kotak"> <strong>00</strong> </span>
                <span class="kotak"><strong>00</strong></span>
                <span class="kotak"><strong>00</strong></span>
                <span class="kotak"><strong>00</strong></span>
              </div>
            </div>
          </div>

          <hr />
        </div>

        <table class="table mt-3 mb-4">
          <thead>
            <tr>
              <th scope="col">Varian</th>
              <th scope="col">Harga</th>
              <th scope="col">Jumlah</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td><span class="varian">Varian</span></td>
              <td><span class="harga">Rp 10.000 / 1000 Meter</span></td>
              <td>
                <controlQuantity
                  :jumlah="jumlah"
                  @tambah="tambahQuantity"
                  @kurang="kurangQuantity"
                />
              </td>
            </tr>
          </tbody>
        </table>
        <hr />
        <p>
          Voucher Promo: <span class="banner-promo ml-4">Banner Promo</span>
        </p>
      </div>
      <div class="col-md-3">
        <div class="card shadow-sm font-smaller">
          <div class="card-body">
            <p style="color: #65af98"><strong>Ready Stock</strong></p>
            <p style="margin-bottom: 0 !important">
              Minimal Order (MOQ): 100 Meter
            </p>
            <p style="margin-bottom: 0 !important">
              Kelipatan Order: 100 Meter
            </p>
            <p>
              <span class="gray"> Total Kuantitas:</span>
              <span class="float-right"> <strong>0 Meter</strong> </span>
            </p>
            <hr />
            <p>
              <span class="gray"> Total Harga</span>

              <span class="float-right"> <strong> Rp. 00.000 </strong></span>
            </p>
            <button class="btn btn-main btn-block">
              <strong>Beli Sekarang</strong>
            </button>
            <button class="btn btn-secondary btn-block">
              <strong>
                <i class="fas fa-cart-plus"></i> Masukkan Keranjang</strong
              >
            </button>
          </div>
        </div>

        <div class="card shadow-sm mt-4 font-smaller">
          <div class="card-body" style="padding-bottom: 0 !important">
            <p>Pengiriman</p>
            <p style="margin-bottom: 5px !important">
              <img src="assets/img/buildings.png" alt="building" />
              <span class="gray ml-1">Dikirim dari</span> Kab. Bandung
            </p>
            <div>
              <div class="float-left mr-1">
                <img src="assets/img/truck.png" alt="truck" />
              </div>
              <div>
                <span class="gray ml-1">Pengiriman ke</span> Kota Jakarta <br />
                <span class="gray ml-1">Ongkos Kirim</span>
              </div>
            </div>
            <p class="float-right">
              <strong>Rp.00.000</strong>
            </p>
            <p style="clear: both" class="float-right">
              <span class="gray"
                >Kargo JNE Trucking (JTR)
                <span class="main-color" style="cursor: pointer">Ubah</span>
              </span>
            </p>
          </div>
          <div
            class="card-footer"
            style="background-color: white; padding: 10px 10px 0 0 !important"
          >
            <p class="float-right">
              <span class="gray">Estimasi tiba 12/Des - 15/Des</span>
            </p>
          </div>
        </div>
      </div>
    </div>
    <hr />
    <!-- Owner Produk  -->
    <div class="row">
      <div class="col-md-9">
        <div class="card shadow-sm" style="border-radius: 20px">
          <div class="card-body">
            <div style="height: 80px" class="float-left">
              <img
                src="assets/img/pp-seller.png"
                alt="pp seller"
                class="mr-2"
              />
            </div>
            <div class="float-right">
              <ul class="nav mt-3">
                <li class="nav-item border-left">
                  <a class="nav-link active" href="#">
                    <img src="assets/img/unlinkIcon.png" /> Copy Link</a
                  >
                </li>
                <li class="nav-item border-left">
                  <a class="nav-link" href="#">
                    <img src="assets/img/shareIcon.png" /> Share</a
                  >
                </li>
                <li class="nav-item border-left">
                  <a class="nav-link" href="#">
                    <img src="assets/img/favoriteIcon.png" /> Favorit (0,0RB)</a
                  >
                </li>
              </ul>
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
              <span class="gray">Kab. Bandung </span> <br />
              <i class="fas fa-star main-color"> </i>
              <span class="gray"> 5 (100 Ulasan)</span>
            </p>
          </div>
        </div>
      </div>
    </div>

    <!-- Detail Produk -->
    <detailProduk />

    <!-- List Produk -->
    <h5 class="mt-4"><strong>Produk Populer Packer</strong></h5>
    <div class="row mt-4">
      <div
        class="col-sm-6 col-md-4 col-lg-2 mt-3"
        style="padding: 0px !important; margin: 0px 15px 0px 15px !important"
        v-for="produk in listProduk"
        :key="produk.id"
      >
        <div class="card shadow-sm" style="width: 100%">
          <img
            class="card-img-top"
            src="assets/img/produk.jpg"
            alt="Card image cap"
          />
          <div class="card-body">
            <h5 class="card-title">{{ produk.nama }}</h5>
            <h5>
              <strong>Rp {{ produk.harga }}</strong>
            </h5>
            <p class="card-text">
              MOQ: 00 Meter <br /><i class="fas fa-star main-color"></i>
              <span class="gray"> (00) | Terjual 00</span>
            </p>
          </div>
          <div
            class="card-footer"
            style="
              background-color: white;
              padding: 10px 10px 0px 10px !important;
            "
          >
            <p class="font-smaller gray">Kab. Bandung</p>
          </div>
        </div>
      </div>
    </div>

    <h5 class="mt-4"><strong>Produk Terakhir Dilihat</strong></h5>
    <div class="row mt-4">
      <div
        class="col-sm-6 col-md-4 col-lg-2 mt-3"
        style="padding: 0px !important; margin: 0px 15px 0px 15px !important"
        v-for="produk in listProduk"
        :key="produk.id"
      >
        <div class="card shadow-sm" style="width: 100%">
          <img
            class="card-img-top"
            src="assets/img/produk.jpg"
            alt="Card image cap"
          />
          <div class="card-body">
            <h5 class="card-title">{{ produk.nama }}</h5>
            <h5>
              <strong>Rp {{ produk.harga }}</strong>
            </h5>
            <p class="card-text">
              MOQ: 00 Meter <br /><i class="fas fa-star main-color"></i>
              <span class="gray"> (00) | Terjual 00</span>
            </p>
          </div>
          <div
            class="card-footer"
            style="
              background-color: white;
              padding: 10px 10px 0px 10px !important;
            "
          >
            <p class="font-smaller gray">Kab. Bandung</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import listProduk from "../produk.json";
export default {
  layout: "dashboard",
  data() {
    return {
      listProduk,
      jumlah: 0,
    };
  },
  methods: {
    tambahQuantity() {
      let jumlah = this.jumlah++;
      return jumlah;
    },
    kurangQuantity() {
      if (this.jumlah > 0) {
        let kurang = this.jumlah--;
        return kurang;
      }
    },
  },
};
</script>

<style scoped>
.card-body {
  padding: 10px !important;
}
.col-md-6 {
  padding-left: 0px !important;
}

.foto-produk {
  max-width: 400px !important;
}

.img-list {
  border-radius: 10px;
  width: 60px;
  height: 60px;
}

.kotak {
  border-radius: 10px 10px 10px 0px;
  padding: 3px 10px 3px 10px;
  background-color: #f9be00;
}

.kotak-2 {
  font-size: 10px;
}

.varian {
  border-radius: 10px;
  background-color: #d5d5df;
  padding: 5px 20px 5px 20px;
}
.harga {
  border-radius: 10px;
  background-color: #e7e7ee;
  padding: 5px 20px 5px 20px;
}
.banner-promo {
  border-radius: 8px;
  padding: 10px 40px 10px 10px;
  background-color: #46d5b2;
}
.btn-main {
  color: white;
  background-color: #f9be00;
}

.font-smaller {
  font-size: 15px;
}

.card-produk {
  width: 100px;
}
</style>
