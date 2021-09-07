<template>
  <footer id="footer" class="pt-5 pb-3 bg-lighter">
    <b-container>
      <b-row>
        <b-col sm="12" md="6" lg="3" class="mb-3" order-md="1" order-lg="1">
          <img :src="imgLogo" alt="SIRUS" class="w-100 mb-3" />
          <p class="m-0">Kami merupakan sebuah layanan digital yang bergerak dalam dunia kesehatan untuk masyarakat Ngawi demi penanganan COVID-19 yang optimal.</p>
        </b-col>
        <b-col sm="12" md="6" lg="3" class="mb-3" order-md="4" order-lg="2">
          <div class="widget-title">
            <h3>Tentang Kami</h3>
          </div>
          <ul class="nav flex-column">
            <li class="nav-item"><a class="nav-link" href="#" @click.prevent>Tentang Kami</a></li>
            <li class="nav-item"><a class="nav-link" href="#" @click.prevent>Medical Checkup Gratis</a></li>
            <li class="nav-item"><a class="nav-link" href="#" @click.prevent>Tes Usap Gratis</a></li>
            <li class="nav-item"><a class="nav-link" href="#" @click.prevent>Swab Test Gratis</a></li>
          </ul>
        </b-col>
        <b-col sm="12" md="6" lg="3" class="mb-3" order-md="4" order-lg="3">
          <div class="widget-title">
            <h3>Layanan Kami</h3>
          </div>
          <ul class="nav flex-column">
            <li class="nav-item"><router-link class="nav-link" to="/cek-oksigen">Cek Data Oksigen</router-link></li>
            <li class="nav-item"><router-link class="nav-link" to="/cek-vaksinasi">Cek Data Vaksinasi</router-link></li>
            <li class="nav-item"><router-link class="nav-link" to="/cek-ranap">Cek Data Kamar Ranap</router-link></li>
            <li class="nav-item"><a href="#" class="nav-link" @click.prevent>Cek Jadwal Dokter</a></li>
            <li class="nav-item"><a href="#" class="nav-link" @click.prevent>Cek Jadwal Pemeriksaan</a></li>
            <li class="nav-item"><a href="#" class="nav-link" @click.prevent>Jadwalkan Periksa</a></li>
            <li class="nav-item"><a href="#" class="nav-link" @click.prevent>Ambil Obat</a></li>
          </ul>
        </b-col>
        <b-col sm="12" md="6" lg="3" order-sm="2" order-md="4">
          <div class="widget-title">
            <h3>Berlangganan Yuk!</h3>
          </div>
          <p>Daftarkan alamat surat elektronik anda untuk mendapatkan informasi terbaru seputar layanan kesehatan di Ngawi tanpa harus bolak-balik ke situs ini.</p>

          <form @submit.prevent>

            <div class="form-group form-floating-alt form-floating">
              <input id="email" type="email" class="form-control" placeholder="Mis: admin@sirus.com" />
              <label for="email">Masukkan email anda</label>
            </div>

            <b-button block variant="primary">Kirimkan Email!</b-button>

          </form>
        </b-col>
      </b-row>
      <b-row class="pt-3 mt-3 border-top">
        <b-col md="6">
          <p class="m-0">Hak cipta 2021 <router-link to="/">SIRUS</router-link>.</p>
        </b-col>
      </b-row>
    </b-container>
  </footer>
</template>

<script>
import imgLogos from '../static/brands/logo-color-alt.svg'

export default {
  data: () => ({
    imgLogo: imgLogos,

  }),
}
</script>

<style lang="scss">
footer {
  a {
    color: var(--dark);
  }

  .nav-link {
    padding-left: 0;
    padding-right: 0;

    &:before {
      content: "\f054";
      font-family: 'Font Awesome 5 Free';
      font-weight: 900;
      margin-right: .5rem;
      color: var(--primary);
    }
  }
}
.widget-title {
  border-bottom: 1px solid #ddd;
  position: relative;
  display: flex;
  margin-bottom: 1rem;

  h1, h2, h3, h4, h5, h6 {
    font-size: 1rem;
    font-weight: bolder;
    padding: .25rem 0;
    border-bottom: 3px solid var(--primary);
    margin-bottom: -.15rem;
  }
}
</style>
