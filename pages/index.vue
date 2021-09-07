<template>
  <div id="home">
    <header id="masthead" class="bg-white">
      <TopNav />

      <b-container class="py-5">
        <b-row class="py-5">
          <b-col md="7">
            <router-link to="/cek-ranap" class="new-feature">
              <div class="new">Baru!</div>
              <div class="wrapper">Cek data keterisian rumah sakit atau puskesmas</div>
            </router-link>
            <h3>Pelayanan Prima, Keluarga Bahagia</h3>
            <p class="text-muted">Kami memberikan pelayanan konsultasi, bantuan tabung oksigen dan isinya, data informasi rumah sakit dan juga bantuan informasi kesehatan yang dapat digunakan masyarakat Ngawi yang sedang terkena covid dan atau ingin mencari rujukan.</p>

            <b-button variant="outline-primary">Cek Kamar</b-button>
            <b-button variant="primary">Cek Layanan</b-button>
          </b-col>
          <b-col md="5" class="d-none d-md-none d-lg-inline">
            <b-img :src="imgHuman" class="w-100" />
          </b-col>
        </b-row>
      </b-container>
    </header>

    <section id="featured">
      <b-container class="py-5">
        <b-row>
          <b-col cols="6" class="mb-3" md="3">

            <div class="featured">
              <div class="icon"><i class="fas fa-bolt"></i></div>
              <div class="content">
                <h3>Pelayanan Cepat</h3>
                <div class="text-muted">Kami memberikan pelayanan yang cepat dalam kurun waktu 3 jam sudah kami bantu antar obatnya.</div>
              </div>
            </div>

          </b-col>
          <b-col cols="6" class="mb-3" md="3">

            <div class="featured">
              <div class="icon"><i class="fas fa-sync"></i></div>
              <div class="content">
                <h3>Data Akurat</h3>
                <div class="text-muted">Data kamar yang kami berikan merupakan data yang akurat dari tim kami.</div>
              </div>
            </div>

          </b-col>
          <b-col cols="6" class="mb-3" md="3">

            <div class="featured">
              <div class="icon"><i class="fas fa-check"></i></div>
              <div class="content">
                <h3>Dokter Profesional</h3>
                <div class="text-muted">Dokter kami siap sedia membantu anda sewaktu-waktu dan memberikan solusi terbaik untuk kesehatan anda.</div>
              </div>
            </div>

          </b-col>
          <b-col cols="6" class="mb-3" md="3">

            <div class="featured">
              <div class="icon"><i class="fas fa-clock"></i></div>
              <div class="content">
                <h3>24/7 Hari Full</h3>
                <div class="text-muted">Dokter kami siap sedia membantu anda sepanjang hari untuk membantu anda dalam masalah kesehatan.</div>
              </div>
            </div>

          </b-col>
        </b-row>
      </b-container>
    </section>

  </div>
</template>

<script>
import imgHead from '../static/bg-header-home.jpg'
import imgPer from '../static/person.png'

export default {
  name: 'HomePage',
  data: () => ({
    imgHeader: imgHead,
    imgHuman: imgPer,

    items: [
      {
        daerah: 'Sine',
        puskesmas: 'Puskesmas Sine',
        jumlah: 12,
        terisi: 12,
      },
      {
        daerah: 'Ngrambe',
        puskesmas: 'Puskesmas Ngrambe',
        jumlah: 12,
        terisi: 11,
      },
      {
        daerah: 'Jogorogo',
        puskesmas: 'Puskesmas Jogorogo',
        jumlah: 10,
        terisi: 7,
      },
      {
        daerah: 'Kendal',
        puskesmas: 'Puskesmas Kendal',
        jumlah: 10,
        terisi: 4,
      },
      {
        daerah: 'Gerih',
        puskesmas: 'Puskesmas Widodaren',
        jumlah: 15,
        terisi: 7,
      },
      {
        daerah: 'Geneng',
        puskesmas: 'Puskesmas Geneng',
        jumlah: 12,
        terisi: 5,
      },
      {
        daerah: 'Kwadungan',
        puskesmas: 'Puskesmas Kwadungan',
        jumlah: 12,
        terisi: 2,
      },
      {
        daerah: 'Pangkur',
        puskesmas: 'Puskesmas Pangkur',
        jumlah: 12,
        terisi: 0,
      },
      {
        daerah: 'Karangjati',
        puskesmas: 'Puskesmas Karangjati',
        jumlah: 15,
        terisi: 5,
      },
      {
        daerah: 'Bringin',
        puskesmas: 'Puskesmas Bringin',
        jumlah: 5,
        terisi: 5,
      },
      {
        daerah: 'Padas',
        puskesmas: 'Puskesmas Padas',
        jumlah: 20,
        terisi: 5,
      },
      {
        daerah: 'Kasreman',
        puskesmas: 'Puskesmas Kasreman',
        jumlah: 15,
        terisi: 8,
      },
      {
        daerah: 'Ngawi',
        puskesmas: 'Puskesmas Ngawi',
        jumlah: 21,
        terisi: 6,
      },
      {
        daerah: 'Ngawi',
        puskesmas: 'Puskesmas Ngawi Purba',
        jumlah: 11,
        terisi: 8,
      },
      {
        daerah: 'Paron',
        puskesmas: 'Puskesmas Paron',
        jumlah: 17,
        terisi: 8,
      },
      {
        daerah: 'Teguhan',
        puskesmas: 'Puskesmas Teguhan',
        jumlah: 16,
        terisi: 15,
      },
      {
        daerah: 'Kedunggalar',
        puskesmas: 'Puskesmas Kedunggalar',
        jumlah: 14,
        terisi: 10,
      },
      {
        daerah: 'Kedunggalar',
        puskesmas: 'Puskesmas Gemarang',
        jumlah: 13,
        terisi: 10,
      },
      {
        daerah: 'Pitu',
        puskesmas: 'Puskesmas Pitu',
        jumlah: 11,
        terisi: 10,
      },
      {
        daerah: 'Widodaren',
        puskesmas: 'Puskesmas Walikukun',
        jumlah: 20,
        terisi: 10,
      },
      {
        daerah: 'Widodaren',
        puskesmas: 'Puskesmas Kauman',
        jumlah: 11,
        terisi: 10,
      },
      {
        daerah: 'Mantingan',
        puskesmas: 'Puskesmas Mantingan',
        jumlah: 12,
        terisi: 8,
      },
      {
        daerah: 'Mantingan',
        puskesmas: 'Puskesmas Tambakboyo',
        jumlah: 10,
        terisi: 3,
      },
      {
        daerah: 'Karanganyar',
        puskesmas: 'Puskesmas Karanganyar',
        jumlah: 8,
        terisi: 1,
      },
    ]
  }),
  head: {
    title: 'SIRUS &mdash; Sistem Informasi Rumah Sakit',
  },
}
</script>

<style lang="scss">
body {
  overflow-x: hidden;
}

.new-feature {
  display: flex;
  color: dark;
  border-radius: 50rem;
  margin-bottom: 1rem;
  align-items: center;
  text-decoration: none;
  background: var(--light);
  padding: .5rem;

  @media screen and (max-width: 768px) {
    padding: .5rem;
  }

  &:hover {
    text-decoration: none;
  }

  .new {
    margin: 0;
    padding: .5rem 1rem;
    background: var(--success);
    border-radius: 50rem;
    color: white;
  }

  .wrapper {
    color: var(--dark);
    padding: 0 1rem;
  }
}

#masthead {
  background-size: cover;
  position: relative;

  svg {
      z-index: 3;
      position: relative;
  }

  h3 {
    font-family: Montserrat, Arial, Helvetica, sans-serif;
    font-weight: 900;
    font-size: 2.75rem;
  }
  p {
    font-size: 1.15rem;
  }
}

.featured {
  .icon {
    background: rgba(0,0,0,.05);
    position: relative;
    width: 3.5rem;
    display: flex;
    align-items: center;
    justify-content: center;
    height: 3.5rem;
    border-radius: 5rem;
    color: var(--primary);
    font-size: 1.5rem;
    margin-bottom: .5rem;
  }
}
</style>
