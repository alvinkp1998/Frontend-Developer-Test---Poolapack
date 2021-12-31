<template>
  <div>
    <div class="float-right mb-3 top">
      <ul class="nav mr-3 mt-3">
        <li class="nav-item">
          <img src="assets/img/clipboard.png" alt="" class="icon" />
          <span> Sampel </span>
        </li>
        <li class="nav-item ml-3">
          <img src="assets/img/heart.png" alt="" class="icon" />
          <span> Wishlist</span>
        </li>
        <li class="nav-item ml-4">
          <img src="assets/img/3d-square.png" alt="" class="icon" />
        </li>
        <li class="nav-item ml-3">
          <img src="assets/img/sms-notification.png" alt="" class="icon" />
        </li>
        <li class="nav-item ml-4">
          <img src="assets/img/user-square.png" alt="" class="icon" />
          <span> User </span>
        </li>
      </ul>
    </div>
    <div style="clear: both">
      <hr />
    </div>

    <ul class="nav d-flex align-items-center">
      <li class="nav-item">
        <img src="assets/img/logo-2.png" alt="logo" class="logo" />
      </li>
      <li class="nav-item mr-5">
        <a class="nav-link" href="#"
          >Kategori <span><i class="fas fa-chevron-down ml-1"></i> </span
        ></a>
      </li>
      <li class="nav-item pt-3 ml-auto">
        <div class="input-group mb-3 d-flex">
          <div class="input-group-append">
            <input
              type="text"
              class="form-control"
              placeholder="Search..."
              size="60"
            />
            <button class="btn btn-main bg-main">
              <i class="fas fa-search pl-2 pr-2"></i>
            </button>
          </div>
        </div>
      </li>
      <li class="nav-item ml-4">
        <img
          src="assets/img/shopping-cart.png"
          alt="shopping-cart"
          class="icon"
          style="cursor: pointer"
          @click="$router.push('/keranjang')"
        />
      </li>
    </ul>

    <div class="nav-content mt-4">
      <nav class="nav">
        <a class="nav-link active border-left padding-left-right" href="#"
          >Tentang Kami</a
        >
        <a class="nav-link border-left padding-left-right" href="#">
          Cara Belanja</a
        >
        <a class="nav-link border-left padding-left-right" href="#">Referral</a>
        <a class="nav-link border-left padding-left-right" href="#">Blog</a>
        <a class="nav-link border-left padding-left-right" href="#">
          <strong>RFQ </strong>
        </a>
      </nav>
    </div>

    <hr class="shadow" />
  </div>
</template>

<style scoped>
.icon {
  width: 30px;
  height: 30px;
}

.top {
  margin-right: 50px;
}

.logo {
  width: 100%;
  height: 70px;
}

.padding-left-right {
  padding-left: 30px !important;
  padding-right: 30px !important;
}

.nav-link {
  padding-top: 0 !important;
  padding-bottom: 0 !important;
}
</style>
