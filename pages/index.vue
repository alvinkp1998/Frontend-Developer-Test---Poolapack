<template>
  <div>
    <div class="main-container">
      <header>
        <img src="assets/img/logo.png" alt="logo" class="float-left" />
        <h3 class="float-right login">Masuk Akun</h3>
      </header>
      <main class="mt-5 d-flex justify-content-center">
        <div class="row align-items-center">
          <div class="col-md-6 text-center pr-5">
            <img src="assets/img/jumbotron.jpg" alt="jumbotron" />
            <div class="text-center">
              <h3>Kemudahan mencari bahan baku</h3>
              <p>One Click to Industry</p>
            </div>
          </div>
          <div class="col-md-6 mt-5 pl-4">
            <div class="card shadow">
              <div class="card-body p-4">
                <h3 style="font-weight: 700; font-size: 24px">Masuk Akun</h3>
                <p class="gray">
                  Isi email untuk masuk atau
                  <span class="main-color">daftarkan akun </span>
                </p>
                <form>
                  <div class="form-group">
                    <label for="email">Email</label>
                    <input
                      type="email"
                      class="form-control"
                      id="email"
                      placeholder="Masukkan email"
                    />
                  </div>
                  <div class="form-group">
                    <label for="password">Kata Sandi</label>
                    <div class="input-group">
                      <input
                        id="password"
                        :type="showPassword ? 'password' : 'text'"
                        class="form-control"
                        placeholder="Masukkan kata sandi"
                        required
                      />
                      <div class="input-group-append eye">
                        <span class="input-group-text bg-white"
                          ><i
                            :class="
                              showPassword ? 'fas fa-eye-slash' : 'fas fa-eye'
                            "
                            @click="showPassword = !showPassword"
                          ></i
                        ></span>
                      </div>
                    </div>

                    <small id="emailHelp" class="form-text text-muted"
                      >Kombinasi angka, huruf besar dan huruf kecil</small
                    >
                  </div>
                  <p class="gray">
                    Lupa sandi? Silahkan ke halaman
                    <span class="main-color">lupa password </span>
                  </p>

                  <button
                    type="button"
                    class="btn btn-main btn-block"
                    @click="toProduct"
                  >
                    Selanjutnya
                  </button>
                </form>
              </div>
            </div>
          </div>
        </div>
      </main>
      <footer class="navbar fixed-bottom">
        <div class="float-left">
          <p>&copy; 2021 - Poolapack.com</p>
        </div>
        <div class="float-right second-color">
          <span class="mr-3 pointer">Hubungi Kami</span>
          <span class="mr-3 pointer">Laporkan Masalah</span>
          <span class="mr-3 pointer">Karir</span>
        </div>
      </footer>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showPassword: true,
    };
  },
  methods: {
    toProduct() {
      this.$router.push("/produk");
    },
  },
};
</script>

<style scoped>
header {
  padding: 50px;
}

.card {
  border-radius: 10px;
  width: 600px;
}
.login {
  font-weight: 700;
  font-size: 24px;
  cursor: pointer;
}

.main-color {
  color: #f9be00;
}
.second-color {
  color: #4b1412;
}
.btn-main {
  color: white;
  background-color: #f9be00;
}

.pointer {
  cursor: pointer;
}

footer {
  padding: 0px 50px 15px 50px;
  bottom: 0;
}
</style>
