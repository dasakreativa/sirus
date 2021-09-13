<template>
  <div id="vaksinasi">
    <header id="masthead-vaksinasi">
      <TopNav />
    </header>

    <section id="breadcrumbs" class="py-3 bg-light">
      <b-container>
        <b-breadcrumb class="bg-light m-0">
          <b-breadcrumb-item to="/">Beranda</b-breadcrumb-item>
          <b-breadcrumb-item active>Data Penyedia Oksigen</b-breadcrumb-item>
        </b-breadcrumb>
      </b-container>
    </section>

    <b-container class="py-5">
      <h3 class="text-montserrat">Data Penyedia Oksigen</h3>
      <p class="text-muted">Daftar tempat penyedia oksigen di Ngawi.</p>

      <b-row>
        <b-col v-for="(data, i) in this.show" :key="i" class="mb-3" md="4">
          <a target="_blank" class="card card-body card-alamat" :href="`https://www.google.com/search?q=${data.alamat}`">
            <b-row>
              <b-col cols="3">
                <svg width="100%" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1080 1080"><g style="opacity:0.25"><circle cx="540" cy="540" r="540" style="fill:#3171e0"/></g><path d="M501.14,298.45c.16-.19,55.86-64.79,143.06-16.47,27.32,15.14,50.25,39.78,73.28,64.55,43.11,46.34,86.69,93.19,157.63,64.14l0,.07a11.88,11.88,0,0,1,9.22-.11,12.17,12.17,0,0,1-.17,22.59h0c-86.27,35.32-135.56-17.66-184.32-70.08-21.63-23.26-43.16-46.4-67.33-59.79C562.32,264.45,519.13,314.65,519,314.79Z" style="fill-rule:evenodd"/><polygon points="518.13 240.46 549.51 253.12 525.34 314.01 493.95 301.35 518.13 240.46" style="fill:#3171e0;fill-rule:evenodd"/><path d="M520.82,233.68,559,249.08l-29.57,74.46-44.84-18.09L514.1,231l6.72,2.71Zm19.26,23.49L522.16,250l-18.78,47.32,17.91,7.22Z" style="fill-rule:evenodd"/><path d="M425.26,272.42l169.61,68.4a38.29,38.29,0,0,1,21,49.49L572,500.84l-239.74-96.7,43.89-110.53A37.77,37.77,0,0,1,425.26,272.42Z" style="fill:#3171e0;fill-rule:evenodd"/><polygon points="241.94 631.61 481.67 728.31 572.01 500.84 332.27 404.13 241.94 631.61" style="fill:#e6e6e6;fill-rule:evenodd"/><path d="M219.07,791.61,388.67,860a37.78,37.78,0,0,0,49.1-21.2l43.9-110.52-239.74-96.7L198,742.13A38.26,38.26,0,0,0,219.07,791.61Z" style="fill:#3171e0;fill-rule:evenodd"/><path d="M507,226h0a13.83,13.83,0,0,1,18-7.76l34.75,14a14,14,0,0,1,7.7,18.11h0a13.84,13.84,0,0,1-18,7.76l-34.76-14A14,14,0,0,1,507,226Z" style="fill:#633;fill-rule:evenodd"/><path d="M500.28,223.3a21.16,21.16,0,0,1,11.29-11.61,20.81,20.81,0,0,1,16.13-.23l34.75,14A21.1,21.1,0,0,1,574,236.83a21.24,21.24,0,0,1-11.05,27.91,20.9,20.9,0,0,1-16.11.21l-34.78-14a21.39,21.39,0,0,1-11.74-27.63Zm13.5,5.43a6.66,6.66,0,0,0,.07,5.06,6.57,6.57,0,0,0,3.58,3.54l34.75,14a6.49,6.49,0,0,0,5-.06,6.56,6.56,0,0,0,3.5-3.59,6.62,6.62,0,0,0-3.64-8.62l-34.75-14a6.58,6.58,0,0,0-8.52,3.68Z" style="fill-rule:evenodd"/><path d="M340.56,530q6.4-16.17,15.23-25.33a53.68,53.68,0,0,1,14.82-10.84A40.74,40.74,0,0,1,387,489.34a54,54,0,0,1,22.68,4.29q21.52,8.69,28.69,28.4t-3.08,45.54q-10.18,25.62-28.75,34.93t-40,.61q-21.74-8.77-28.84-28.32T340.56,530Zm20.56,7.46q-7.14,18-3.19,30.3a26.16,26.16,0,0,0,15.73,17.12,25.69,25.69,0,0,0,23-1.4q11.2-6.18,18.51-24.58,7.23-18.18,3.43-30.09T402.61,512q-12.18-4.92-23.21,1.14T361.12,537.42Z"/><path d="M449.18,634.18l-3.57,9-31.26-12.61a26.43,26.43,0,0,1,6.89-8.4c2.9-2.38,7.84-5,14.84-8.07q8.44-3.66,10.67-5.3a12,12,0,0,0,4.2-5.17,7.66,7.66,0,0,0,.37-5.64,6.25,6.25,0,0,0-3.74-3.5,6,6,0,0,0-5.17,0c-1.57.76-3,2.53-4.31,5.3l-8.5-4.57q4-7.66,9.55-9.44a16.94,16.94,0,0,1,11.84.73q6.88,2.79,9.22,8.41a14.87,14.87,0,0,1,0,11.6,19.51,19.51,0,0,1-3.7,6,28.28,28.28,0,0,1-6.13,5,64.1,64.1,0,0,1-8.4,4.08c-3.93,1.68-6.46,2.8-7.56,3.44a16.83,16.83,0,0,0-2.9,1.95Z"/><path d="M552.78,485.19l.18.06,15,6.07,41.2-103.72a31,31,0,0,0-.33-23.51,30.54,30.54,0,0,0-16.68-16.47l-169.6-68.4a30.21,30.21,0,0,0-23.33.32,30.58,30.58,0,0,0-16.33,16.79L341.72,400.06l149.59,60.33.17.07a7.35,7.35,0,0,1,4,9.53,7.24,7.24,0,0,1-9.45,4.07l-.17-.07L336.32,413.65,251.38,627.53l27,10.89.17.07a7.35,7.35,0,0,1,4,9.52,7.24,7.24,0,0,1-9.44,4.08L273,652l-27-10.89L204.79,744.85a30.89,30.89,0,0,0,.32,23.51,30.4,30.4,0,0,0,16.66,16.46l169.61,68.41a30.16,30.16,0,0,0,23.31-.3A30.68,30.68,0,0,0,431,836.11l41.19-103.72L334.61,676.88l-.17-.07a7.34,7.34,0,0,1-4-9.52,7.25,7.25,0,0,1,9.44-4.08l.18.08L477.64,718.8l84.94-213.88-15-6.06-.17-.07a7.35,7.35,0,0,1-4-9.53,7.23,7.23,0,0,1,9.44-4.07ZM428,265.62,597.57,334a45.07,45.07,0,0,1,24.59,24.28,45.58,45.58,0,0,1,.49,34.72L581.42,496.74,580,500.29l-1.41,3.56-1.41,3.55q-43,108.45-86.1,216.82h0l-46.6,117.32a45.08,45.08,0,0,1-24.1,24.81,44.59,44.59,0,0,1-34.45.46l-169.6-68.41a45.06,45.06,0,0,1-24.61-24.29,45.55,45.55,0,0,1-.47-34.71l41.2-103.72,5.39-13.6,84.95-213.88,5.4-13.6,41.19-103.72a45.13,45.13,0,0,1,24.1-24.82A44.58,44.58,0,0,1,428,265.62Z" style="fill-rule:evenodd"/><path d="M520.89,279.38a29.42,29.42,0,0,1,16.21,38.15,29,29,0,0,1-37.85,16.34A29.44,29.44,0,0,1,483,295.71,29,29,0,0,1,520.89,279.38Z" style="fill:#fff;fill-rule:evenodd"/><path d="M523.59,272.58a36.34,36.34,0,0,1,19.92,19.6,36.81,36.81,0,0,1,.34,28.06,36.42,36.42,0,0,1-19.46,20.09,36,36,0,0,1-27.84.31,36.62,36.62,0,0,1,27-68.06Zm-5.39,13.6a21.68,21.68,0,0,0-16.73.19,21.92,21.92,0,0,0-11.69,12.07,22.21,22.21,0,0,0,.19,16.85,21.79,21.79,0,0,0,40.38-.49,22.12,22.12,0,0,0-.19-16.85A21.88,21.88,0,0,0,518.2,286.18Z" style="fill-rule:evenodd"/><path d="M517.28,288.44h0a4.53,4.53,0,0,1,2.48,5.85l-4.33,10.9a4.45,4.45,0,0,1-5.79,2.49h0a4.51,4.51,0,0,1-2.48-5.84l4.32-10.9A4.47,4.47,0,0,1,517.28,288.44Z" style="fill-rule:evenodd"/></svg>
              </b-col>
              <b-col cols="9">
                <h4 class="h5 text-montserrat">{{ data.nama }} ({{ data.wilayah }})</h4>
                <ul class="list-unstyled mb-0">
                  <li><i class="fas fa-map-marker mr-2"></i>{{ data.alamat }}</li>
                  <li><i class="fas fa-database mr-2"></i>{{ data.stok }} Tersisa</li>
                </ul>
              </b-col>
            </b-row>
          </a>
        </b-col>
      </b-row>
    </b-container>

    <Footer />
  </div>
</template>

<script>
export default {
  name: 'DataOksigen',
  data() {
    return {
      tempat: [
        {
          nama: 'CV. Hargo Dumilah Oksigen',
          wilayah: 'Ngrambe',
          alamat: 'Jl. Pudak, GG. Perkutut, Ngancar, Ngrambe, Ngawi, Jawa Timur',
          stok: 120,
          sisa: 100,
        },
        {
          nama: 'CV. Barokah Anak Agung Perkasa',
          wilayah: 'Widodaren',
          alamat: 'Jl. Raya Ngawi-Solo, Desa Gendingan, Widodaren, Ngawi, Jawa Timur',
          stok: 50,
          sisa: 10,
        },
        {
          nama: 'CV. Barokah Anak Agung Perkasa',
          wilayah: 'Mantingan',
          alamat: 'Jl. Raya Ngawi-Solo, Mantingan, Ngawi, Jawa Timur',
          stok: 50,
          sisa: 10,
        },
        {
          nama: 'Apotek Wahyu Medika',
          wilayah: 'Gerih',
          alamat: 'Guyung, Gerih, Ngawi, Jawa Timur',
          stok: 50,
          sisa: 10,
        },
        {
          nama: 'UD. Oxycal Husada Ngawi',
          wilayah: 'Ngawi',
          alamat: 'Gg. Perkutut, Beran, Ngawi, Jawa Timur',
          stok: 200,
          sisa: 100,
        },
        {
          nama: 'UD. Perkasa Husada Ngawi',
          wilayah: 'Karangjati',
          alamat: 'Jl. Raya Ngawi-Caruban, Legundi, Karangjati, Ngawi, Jawa Timur',
          stok: 143,
          sisa: 100,
        },
        {
          nama: 'PT. Hero Chemical Transindo (Tbk.)',
          wilayah: 'Geneng',
          alamat: 'Jl. Raya Ngawi-Maospati, Klitik, Geneng, Ngawi, Jawa Timur',
          stok: 55,
          sisa: 41,
        },
        {
          nama: 'CV. Paron Jaya Chemical',
          wilayah: 'Paron',
          alamat: 'Jl. Raya Ngawi-Jogorogo, Dadapan, Paron, Ngawi, Jawa Timur',
          stok: 54,
          sisa: 50,
        },
        {
          nama: 'CV. Widodo Putra Tech',
          wilayah: 'Kwadungan',
          alamat: 'Jl. Raya Kwadungan-Geneng, Kwadungan, Ngawi, Jawa Timur',
          stok: 20,
          sisa: 10,
        },
        {
          nama: 'CV. Widodo Putra Tech',
          wilayah: 'Bringin',
          alamat: 'Jl. Raya Kedungprahu-Bringin, Mojo, Bringin, Ngawi, Jawa Timur',
          stok: 25,
          sisa: 15,
        },
        {
          nama: 'Apotek Amanah Medika',
          wilayah: 'Ngawi',
          alamat: 'Karangasri, Ngawi Kota, Ngawi, Jawa Timur',
          stok: 24,
          sisa: 11,
        },
        {
          nama: 'Apotek Waras',
          wilayah: 'Padas',
          alamat: 'Jl. Raya Ngawi-Caruban KM 8, Pacing, Padas, Ngawi, Jawa Timur',
          stok: 22,
          sisa: 15,
        },
        {
          nama: 'SAR MTA Perwakilan Ngawi',
          wilayah: 'Ngrambe',
          alamat: 'Hargomulyo, Ngrambe, Ngawi, Jawa Timur',
          stok: 50,
          sisa: 15,
        },
        {
          nama: 'SAR MTA Cabang Ngawi',
          wilayah: 'Ngawi',
          alamat: 'Beran, Ngawi Kota, Ngawi, Jawa Timur',
          stok: 12,
          sisa: 11,
        },
        {
          nama: 'Rumah Sakit Rahayu Persada',
          wilayah: 'Karangjati',
          alamat: 'Legundi (Barat Perbatasan Ngawi-Madiun), Karangjati, Ngawi, Jawa Timur',
          stok: 13,
          sisa: 12,
        },
      ],
      show: [],
      showdata: 6,
    };
  },
  methods: {
    getData() {
      this.show = this.tempat.slice(0, 6);
    },
    getNextUser() {
      window.onscroll = () => {
        console.log(document.documentElement.scrollTop, window.innerHeight, document.innerHeight, document.documentElement.offsetHeight);
        const bottomOfWindow = document.documentElement.scrollTop + window.innerHeight === document.documentElement.offsetHeight;
        if (bottomOfWindow) {
          this.show = this.tempat.slice(0, this.showdata + 6);
          this.showdata = this.showdata + 6;
        }
      }
    }
  },
  beforeMount() {
    this.getData();
  },
  head: {
    title: "Cek Ketersediaan Oksigen - Sistem Informasi Rumah Sakit"
  },
  mounted() {
    this.getNextUser();
  }
}
</script>

<style lang="scss">
.card-alamat {
  box-shadow: 0 4px 16px 0 rgba(33,37,41, 0.1) !important;
  text-decoration: none;
  color: var(--dark);
  transition: all .2s;

  &:hover {
    text-decoration: none;
    box-shadow: none;
    color: var(--dark);
    border-color: rgb(49, 113, 224) !important;
    background: rgba(49, 113, 224, .1);
  }
  &:focus, &:active {
    background: rgb(49, 113, 224);
    color: #fff !important;
    p {
      color: rgb(255, 250, 240);
    }
  }
}
</style>
