<template>
  <div>
    <div class="container">
      <div class="card" style="margin-top: 80px">
        <div class="card-body">
          <div
            class="row"
            style="
              position: absolute;
              margin-top: -50px;
              width: 100%;
              margin-left: 100px;
            "
          >
            >
            <div class="col-3">
              <button class="btn btn-main btn-block">
                <strong>Detail Produk</strong>
              </button>
            </div>
            <div class="col-3">
              <button class="btn btn-inactive btn-block">
                <strong>Ulasan</strong>
              </button>
            </div>
            <div class="col-3">
              <button class="btn btn-inactive btn-block">
                <strong>Profil Packer</strong>
              </button>
            </div>
          </div>
          <h5 class="mt-4"><strong>Detail</strong></h5>
          <table
            class="table table-bordered text-center mt-3"
            style="width: 350px"
          >
            <thead>
              <tr class="table-color">
                <th scope="col" style="width: 130px">Gramasi</th>
                <td scope="col">100.000</td>
              </tr>
            </thead>
            <tbody>
              <tr>
                <th scope="row">Lebar Kain</th>
                <td>150</td>
              </tr>
              <tr class="table-color">
                <th scope="row">Bahan</th>
                <td>100% Cotton</td>
              </tr>
              <tr>
                <th scope="row">Teknik</th>
                <td>Lembut, tahan lama, tidak mudah berkerut</td>
              </tr>
              <tr class="table-color">
                <th scope="row">Karakter</th>
                <td>Fashion</td>
              </tr>
            </tbody>
          </table>
          <h5 class="pt-2"><strong>Deskripsi</strong></h5>
          <p>
            Bahan polyester adalah salah satu jenis kain yang dibuat melalui
            tahapan kimia yang cukup panjang sehingga termasuk salah satu jenis
            kain sintetis. Singkatnya, bahan polyester tidak diperoleh secara
            alami dan juga tidak tersedia bebas di alam ini seperti halnya bahan
            wol, katun dan berbagai jenis bahan dari hasil alam lainnya. Bahan
            sintetis hanya bisa diperoleh melalui proses kimia di pabrik.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.table-color {
  background-color: #eef2f5;
}

.btn-main {
  color: white;
  background-color: #f9be00;
  border-radius: 10px;
  padding-top: 15px;
  padding-bottom: 15px;
}

.btn-inactive {
  color: #f9be00;
  background-color: #fef5d9;
  border-radius: 10px;
  padding-top: 15px;
  padding-bottom: 15px;
}
</style>
