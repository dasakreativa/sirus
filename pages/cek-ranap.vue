<template>
  <div id="vaksinasi">
    <header id="masthead-vaksinasi">
      <TopNav />
    </header>

    <section id="ranap">

      <section id="search-container">
        <b-container class="py-5">
          <b-row class="justify-content-center py-3">
            <b-col md="12">
              <h3 class="text-center">Data Keterisian Kamar Puskesmas</h3>
              <DataTables :data="items" />
            </b-col>
          </b-row>
        </b-container>
      </section>
    </section>

    <Footer />

  </div>
</template>


<script>
export default {
  name: 'CekRanap',
  data: () => ({
    items: [
      {
        daerah: 'Sine',
        puskesmas: 'Puskesmas Sine',
        jumlah: 12,
        terisi: 12,
      },
      {
        daerah: 'Ngawi',
        puskesmas: 'RS Umum Widodo Ngawi',
        jumlah: 210,
        terisi: 120,
      },
      {
        daerah: 'Ngawi',
        puskesmas: 'RS Umum Daerah Dr. Soeroto Ngawi',
        jumlah: 250,
        terisi: 145,
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
        daerah: 'Paron',
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
    title: 'Cek Ranap - Sistem Informasi Rumah Sakit',
  },
}
</script>
