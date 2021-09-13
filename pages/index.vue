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

            <b-button variant="outline-primary" to="/cek-ranap">Cek Kamar</b-button>
            <b-button variant="primary" @click="scrollTo('services')">Cek Layanan</b-button>
          </b-col>
          <b-col md="5" class="d-none d-xs-none d-sm-inline">
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
                <div class="text-muted">Kami memberikan pelayanan yang cepat dalam kurun waktu 3 jam untuk pengiriman obat dan tabung oksigen ke rumah anda.</div>
              </div>
            </div>

          </b-col>
          <b-col cols="6" class="mb-3" md="3">

            <div class="featured">
              <div class="icon"><i class="fas fa-sync"></i></div>
              <div class="content">
                <h3>Data Akurat</h3>
                <div class="text-muted">Data kamar yang kami berikan merupakan data yang diperbaharui setiap waktu agar dapat memantau kondisi di sekitar.</div>
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
                <h3>Bekerja Penuh 24/7 Hari</h3>
                <div class="text-muted">Kami selalu bersedia apabila anda sewaktu-waktu anda membutuhkan pertolongan darurat dan sesegera mungkin.</div>
              </div>
            </div>

          </b-col>
        </b-row>
      </b-container>
    </section>

    <section id="services" class="bg-lighter">
      <b-container class="py-5 text-center">
        <h3>Layanan Kami</h3>

        <b-row class="mt-3">
          <b-col lg="3" class="mb-3" md="6">
            <router-link to="/cek-oksigen" class="card card-body shadow-sm border-0">

              <svg height="100px" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1080 1080"><g style="opacity:0.25"><circle cx="540" cy="540" r="540" style="fill:#3171e0"/></g><path d="M501.14,298.45c.16-.19,55.86-64.79,143.06-16.47,27.32,15.14,50.25,39.78,73.28,64.55,43.11,46.34,86.69,93.19,157.63,64.14l0,.07a11.88,11.88,0,0,1,9.22-.11,12.17,12.17,0,0,1-.17,22.59h0c-86.27,35.32-135.56-17.66-184.32-70.08-21.63-23.26-43.16-46.4-67.33-59.79C562.32,264.45,519.13,314.65,519,314.79Z" style="fill-rule:evenodd"/><polygon points="518.13 240.46 549.51 253.12 525.34 314.01 493.95 301.35 518.13 240.46" style="fill:#3171e0;fill-rule:evenodd"/><path d="M520.82,233.68,559,249.08l-29.57,74.46-44.84-18.09L514.1,231l6.72,2.71Zm19.26,23.49L522.16,250l-18.78,47.32,17.91,7.22Z" style="fill-rule:evenodd"/><path d="M425.26,272.42l169.61,68.4a38.29,38.29,0,0,1,21,49.49L572,500.84l-239.74-96.7,43.89-110.53A37.77,37.77,0,0,1,425.26,272.42Z" style="fill:#3171e0;fill-rule:evenodd"/><polygon points="241.94 631.61 481.67 728.31 572.01 500.84 332.27 404.13 241.94 631.61" style="fill:#e6e6e6;fill-rule:evenodd"/><path d="M219.07,791.61,388.67,860a37.78,37.78,0,0,0,49.1-21.2l43.9-110.52-239.74-96.7L198,742.13A38.26,38.26,0,0,0,219.07,791.61Z" style="fill:#3171e0;fill-rule:evenodd"/><path d="M507,226h0a13.83,13.83,0,0,1,18-7.76l34.75,14a14,14,0,0,1,7.7,18.11h0a13.84,13.84,0,0,1-18,7.76l-34.76-14A14,14,0,0,1,507,226Z" style="fill:#633;fill-rule:evenodd"/><path d="M500.28,223.3a21.16,21.16,0,0,1,11.29-11.61,20.81,20.81,0,0,1,16.13-.23l34.75,14A21.1,21.1,0,0,1,574,236.83a21.24,21.24,0,0,1-11.05,27.91,20.9,20.9,0,0,1-16.11.21l-34.78-14a21.39,21.39,0,0,1-11.74-27.63Zm13.5,5.43a6.66,6.66,0,0,0,.07,5.06,6.57,6.57,0,0,0,3.58,3.54l34.75,14a6.49,6.49,0,0,0,5-.06,6.56,6.56,0,0,0,3.5-3.59,6.62,6.62,0,0,0-3.64-8.62l-34.75-14a6.58,6.58,0,0,0-8.52,3.68Z" style="fill-rule:evenodd"/><path d="M340.56,530q6.4-16.17,15.23-25.33a53.68,53.68,0,0,1,14.82-10.84A40.74,40.74,0,0,1,387,489.34a54,54,0,0,1,22.68,4.29q21.52,8.69,28.69,28.4t-3.08,45.54q-10.18,25.62-28.75,34.93t-40,.61q-21.74-8.77-28.84-28.32T340.56,530Zm20.56,7.46q-7.14,18-3.19,30.3a26.16,26.16,0,0,0,15.73,17.12,25.69,25.69,0,0,0,23-1.4q11.2-6.18,18.51-24.58,7.23-18.18,3.43-30.09T402.61,512q-12.18-4.92-23.21,1.14T361.12,537.42Z"/><path d="M449.18,634.18l-3.57,9-31.26-12.61a26.43,26.43,0,0,1,6.89-8.4c2.9-2.38,7.84-5,14.84-8.07q8.44-3.66,10.67-5.3a12,12,0,0,0,4.2-5.17,7.66,7.66,0,0,0,.37-5.64,6.25,6.25,0,0,0-3.74-3.5,6,6,0,0,0-5.17,0c-1.57.76-3,2.53-4.31,5.3l-8.5-4.57q4-7.66,9.55-9.44a16.94,16.94,0,0,1,11.84.73q6.88,2.79,9.22,8.41a14.87,14.87,0,0,1,0,11.6,19.51,19.51,0,0,1-3.7,6,28.28,28.28,0,0,1-6.13,5,64.1,64.1,0,0,1-8.4,4.08c-3.93,1.68-6.46,2.8-7.56,3.44a16.83,16.83,0,0,0-2.9,1.95Z"/><path d="M552.78,485.19l.18.06,15,6.07,41.2-103.72a31,31,0,0,0-.33-23.51,30.54,30.54,0,0,0-16.68-16.47l-169.6-68.4a30.21,30.21,0,0,0-23.33.32,30.58,30.58,0,0,0-16.33,16.79L341.72,400.06l149.59,60.33.17.07a7.35,7.35,0,0,1,4,9.53,7.24,7.24,0,0,1-9.45,4.07l-.17-.07L336.32,413.65,251.38,627.53l27,10.89.17.07a7.35,7.35,0,0,1,4,9.52,7.24,7.24,0,0,1-9.44,4.08L273,652l-27-10.89L204.79,744.85a30.89,30.89,0,0,0,.32,23.51,30.4,30.4,0,0,0,16.66,16.46l169.61,68.41a30.16,30.16,0,0,0,23.31-.3A30.68,30.68,0,0,0,431,836.11l41.19-103.72L334.61,676.88l-.17-.07a7.34,7.34,0,0,1-4-9.52,7.25,7.25,0,0,1,9.44-4.08l.18.08L477.64,718.8l84.94-213.88-15-6.06-.17-.07a7.35,7.35,0,0,1-4-9.53,7.23,7.23,0,0,1,9.44-4.07ZM428,265.62,597.57,334a45.07,45.07,0,0,1,24.59,24.28,45.58,45.58,0,0,1,.49,34.72L581.42,496.74,580,500.29l-1.41,3.56-1.41,3.55q-43,108.45-86.1,216.82h0l-46.6,117.32a45.08,45.08,0,0,1-24.1,24.81,44.59,44.59,0,0,1-34.45.46l-169.6-68.41a45.06,45.06,0,0,1-24.61-24.29,45.55,45.55,0,0,1-.47-34.71l41.2-103.72,5.39-13.6,84.95-213.88,5.4-13.6,41.19-103.72a45.13,45.13,0,0,1,24.1-24.82A44.58,44.58,0,0,1,428,265.62Z" style="fill-rule:evenodd"/><path d="M520.89,279.38a29.42,29.42,0,0,1,16.21,38.15,29,29,0,0,1-37.85,16.34A29.44,29.44,0,0,1,483,295.71,29,29,0,0,1,520.89,279.38Z" style="fill:#fff;fill-rule:evenodd"/><path d="M523.59,272.58a36.34,36.34,0,0,1,19.92,19.6,36.81,36.81,0,0,1,.34,28.06,36.42,36.42,0,0,1-19.46,20.09,36,36,0,0,1-27.84.31,36.62,36.62,0,0,1,27-68.06Zm-5.39,13.6a21.68,21.68,0,0,0-16.73.19,21.92,21.92,0,0,0-11.69,12.07,22.21,22.21,0,0,0,.19,16.85,21.79,21.79,0,0,0,40.38-.49,22.12,22.12,0,0,0-.19-16.85A21.88,21.88,0,0,0,518.2,286.18Z" style="fill-rule:evenodd"/><path d="M517.28,288.44h0a4.53,4.53,0,0,1,2.48,5.85l-4.33,10.9a4.45,4.45,0,0,1-5.79,2.49h0a4.51,4.51,0,0,1-2.48-5.84l4.32-10.9A4.47,4.47,0,0,1,517.28,288.44Z" style="fill-rule:evenodd"/></svg>
              <h3 class="mt-3 h4">Antar Jemput Oksigen</h3>
              <p>Layanan antar jemput oksigen untuk mempersingkat dan mempercepat waktu pertolongan pertama pasien COVID-19</p>

            </router-link>
          </b-col>
          <b-col lg="3" class="mb-3" md="6">
            <router-link to="/" class="card card-body shadow-sm border-0">

              <svg height="100px" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1080 1080"><g style="opacity:0.25"><circle cx="540" cy="540" r="540" style="fill:#3171e0"/></g><path d="M318.52,429.06h-18a19.77,19.77,0,0,1-19.77-19.77v-18A19.77,19.77,0,0,0,261,371.52h0a19.77,19.77,0,0,0-19.77,19.76v18a19.77,19.77,0,0,1-19.77,19.77h-18a19.77,19.77,0,0,0-19.77,19.77h0a19.77,19.77,0,0,0,19.77,19.77h18a19.77,19.77,0,0,1,19.77,19.76v18A19.77,19.77,0,0,0,261,526.14h0a19.77,19.77,0,0,0,19.77-19.77v-18a19.77,19.77,0,0,1,19.77-19.76h18a19.77,19.77,0,0,0,19.77-19.77h0A19.77,19.77,0,0,0,318.52,429.06Z" style="fill:#ef4343;fill-rule:evenodd"/><path d="M261,526.39a20,20,0,0,1-20-20v-18a19.53,19.53,0,0,0-19.52-19.51h-18a20,20,0,0,1,0-40h18A19.54,19.54,0,0,0,241,409.29v-18a20,20,0,0,1,40,0v18a19.55,19.55,0,0,0,19.52,19.52h18a20,20,0,1,1,0,40h-18A19.54,19.54,0,0,0,281,488.36v18A20,20,0,0,1,261,526.39Zm-57.54-97.08a19.52,19.52,0,0,0,0,39h18a20,20,0,0,1,20,20v18a19.52,19.52,0,1,0,39,0v-18a20,20,0,0,1,20-20h18a19.52,19.52,0,1,0,0-39h-18a20,20,0,0,1-20-20v-18a19.52,19.52,0,0,0-39,0v18a20,20,0,0,1-20,20Z"/><path d="M876.56,429.06h-18a19.77,19.77,0,0,1-19.77-19.77v-18A19.77,19.77,0,0,0,819,371.52h0a19.77,19.77,0,0,0-19.77,19.76v18a19.77,19.77,0,0,1-19.77,19.77h-18a19.77,19.77,0,0,0-19.77,19.77h0a19.77,19.77,0,0,0,19.77,19.77h18a19.77,19.77,0,0,1,19.77,19.76v18A19.77,19.77,0,0,0,819,526.14h0a19.77,19.77,0,0,0,19.77-19.77v-18a19.77,19.77,0,0,1,19.77-19.76h18a19.77,19.77,0,0,0,19.77-19.77h0A19.77,19.77,0,0,0,876.56,429.06Z" style="fill:#ef4343;fill-rule:evenodd"/><path d="M819,526.39a20,20,0,0,1-20-20v-18a19.54,19.54,0,0,0-19.52-19.51h-18a20,20,0,1,1,0-40h18A19.55,19.55,0,0,0,799,409.29v-18a20,20,0,0,1,40,0v18a19.54,19.54,0,0,0,19.52,19.52h18a20,20,0,1,1,0,40h-18A19.53,19.53,0,0,0,839,488.36v18A20,20,0,0,1,819,526.39Zm-57.54-97.08a19.52,19.52,0,1,0,0,39h18a20,20,0,0,1,20,20v18a19.52,19.52,0,0,0,39,0v-18a20,20,0,0,1,20-20h18a19.52,19.52,0,1,0,0-39h-18a20,20,0,0,1-20-20v-18a19.52,19.52,0,0,0-39,0v18a20,20,0,0,1-20,20Z"/><path d="M649.52,526.14h-219a83.06,83.06,0,0,1-83-83V340.3a83.06,83.06,0,0,1,83-83h219a83.06,83.06,0,0,1,83,83V443.16A83.06,83.06,0,0,1,649.52,526.14Zm-219-235.73a50,50,0,0,0-49.89,49.89V443.16a50,50,0,0,0,49.89,49.91h219a50,50,0,0,0,49.89-49.91V340.3a50,50,0,0,0-49.89-49.89Z" style="fill:#3171e0"/><path d="M649.52,526.39h-219a83.32,83.32,0,0,1-83.21-83.23V340.3a83.31,83.31,0,0,1,83.21-83.21h219a83.31,83.31,0,0,1,83.21,83.21V443.16A83.32,83.32,0,0,1,649.52,526.39Zm-219-268.8a82.81,82.81,0,0,0-82.71,82.71V443.16a82.82,82.82,0,0,0,82.71,82.73h219a82.82,82.82,0,0,0,82.71-82.73V340.3a82.81,82.81,0,0,0-82.71-82.71Zm219,235.73h-219a50.2,50.2,0,0,1-50.14-50.16V340.3a50.19,50.19,0,0,1,50.14-50.14h219a50.19,50.19,0,0,1,50.14,50.14V443.16A50.2,50.2,0,0,1,649.52,493.32Zm-219-202.66a49.7,49.7,0,0,0-49.64,49.64V443.16a49.71,49.71,0,0,0,49.64,49.66h219a49.71,49.71,0,0,0,49.64-49.66V340.3a49.7,49.7,0,0,0-49.64-49.64Z"/><rect x="162.66" y="400.15" width="754.68" height="422.51" rx="69.49" style="fill:#3171e0"/><path d="M850.9,826.79H229.1a70.64,70.64,0,0,1-70.58-70.56V466.59A70.66,70.66,0,0,1,229.1,396H850.9a70.66,70.66,0,0,1,70.58,70.58V756.23A70.64,70.64,0,0,1,850.9,826.79ZM229.1,404.28a62.38,62.38,0,0,0-62.31,62.31V756.23a62.38,62.38,0,0,0,62.31,62.3H850.9a62.38,62.38,0,0,0,62.31-62.3V466.59a62.38,62.38,0,0,0-62.31-62.31Z"/><circle cx="540" cy="611.41" r="159.41" style="fill:#dae0e8"/><polygon points="617.31 591.64 559.77 591.64 559.77 534.1 520.23 534.1 520.23 591.64 462.69 591.64 462.69 631.18 520.23 631.18 520.23 688.72 559.77 688.72 559.77 631.18 617.31 631.18 617.31 591.64" style="fill:#ef4343;fill-rule:evenodd"/><path d="M560,689H520V631.43H462.44v-40H520V533.85h40v57.54h57.54v40H560Zm-39.54-.5h39V630.93h57.54v-39H559.52V534.35h-39v57.54H462.94v39h57.54Z"/></svg>
              <h3 class="mt-3 h4">Layanan Berobat</h3>
              <p>Layanan Berobat untuk pasien non-COVID19 agar dapat nyaman dan sehat ketika tidak sedang merasakan gejala COVID-19</p>

            </router-link>
          </b-col>
          <b-col lg="3" class="mb-3" md="6">
            <router-link to="/" @click.native="scrollTo('contact')" class="card card-body shadow-sm border-0">

              <svg height="100px" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1080 1080"><g style="opacity:0.25"><circle cx="540" cy="540" r="540" style="fill:#3171e0"/></g><path d="M726.75,376.08V482.45h-189a84.42,84.42,0,0,0-84.22,84.22v44H367.2a51.07,51.07,0,0,0-37.61,16.23l-33.22,34.51c-18.8,19.83-52.28,6.44-52.28-20.86V376.08a82.23,82.23,0,0,1,82.16-82.17H644.84A82,82,0,0,1,726.75,376.08Z" style="fill:#3171e0;fill-rule:evenodd"/><path d="M644.84,287.48H326.25a88.59,88.59,0,0,0-88.6,88.6V640.59a36.27,36.27,0,0,0,23.18,34,38.34,38.34,0,0,0,13.9,2.83A36.36,36.36,0,0,0,301,665.83l33.23-34.51a45.58,45.58,0,0,1,33-14.17h86.28V604.27H367.2a58.84,58.84,0,0,0-42.24,18l-33.23,34.77c-8.24,8.5-18.8,8.5-26.27,5.67-7.21-3.09-14.94-10.3-14.94-22.15V376.08a75.85,75.85,0,0,1,75.73-75.73H644.84a75.63,75.63,0,0,1,75.47,75.73V482.45h12.88V376.08A88.54,88.54,0,0,0,644.84,287.48Z"/><path d="M601.05,386.37H335.21c-6.85,0-12.4-4.89-12.4-10.92h0c0-6,5.55-10.92,12.4-10.92H601.05c6.85,0,12.4,4.89,12.4,10.92h0C613.45,381.48,607.9,386.37,601.05,386.37Z"/><path d="M601.05,456.59H335.21c-6.85,0-12.4-4.89-12.4-10.93h0c0-6,5.55-10.92,12.4-10.92H601.05c6.85,0,12.4,4.89,12.4,10.92h0C613.45,451.7,607.9,456.59,601.05,456.59Z"/><path d="M775.38,505.59H537.78a61.19,61.19,0,0,0-61.19,61.19V680.59a61.2,61.2,0,0,0,61.19,61.19h207a39,39,0,0,1,28.16,12l24.69,25.84c14.09,14.75,39,4.78,39-15.63V566.78A61.18,61.18,0,0,0,775.38,505.59Z" style="fill:#e6e6e6;fill-rule:evenodd"/><path d="M813.72,792.52a28,28,0,0,1-20.3-8.86l-24.7-25.85a33.32,33.32,0,0,0-24-10.24h-207a67.07,67.07,0,0,1-67-67V566.78a67.06,67.06,0,0,1,67-67h237.6a67,67,0,0,1,67,67V764a27.92,27.92,0,0,1-17.84,26.37A29,29,0,0,1,813.72,792.52ZM537.79,511.38a55.46,55.46,0,0,0-55.4,55.4V680.59a55.46,55.46,0,0,0,55.4,55.4h207a44.92,44.92,0,0,1,32.34,13.82l24.69,25.84a16.82,16.82,0,0,0,29-11.62V566.78a55.46,55.46,0,0,0-55.39-55.4Z"/><rect x="322.81" y="504.96" width="106.59" height="21.84" rx="0.42"/><circle cx="580.01" cy="624.09" r="18.63"/><circle cx="656.58" cy="624.09" r="18.63"/><circle cx="733.16" cy="624.09" r="18.63"/></svg>
              <h3 class="mt-3 h4">Layanan Konsultasi</h3>
              <p>Layanan Konsultasi Gratis kepada seluruh warga Ngawi secara daring.</p>

            </router-link>
          </b-col>
          <b-col lg="3" class="mb-3" md="6">
            <router-link to="/" class="card card-body shadow-sm border-0">

              <svg height="100px" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1080 1080"><g style="opacity:0.25"><circle cx="540" cy="540" r="540" style="fill:#3171e0"/></g><path d="M243.94,713h0a144,144,0,0,0,203.66,0L771.32,389.24a144,144,0,0,0,0-203.66h0a144,144,0,0,0-203.67,0L243.94,509.3A144,144,0,0,0,243.94,713Z" style="fill:#3171e0;fill-rule:evenodd"/><path d="M345.77,762.64a150.5,150.5,0,0,1-107.13-44.38h0a151.5,151.5,0,0,1,0-214.27L562.35,180.28A151.51,151.51,0,1,1,776.62,394.55L452.91,718.26A150.53,150.53,0,0,1,345.77,762.64ZM669.48,151A136,136,0,0,0,573,190.89L249.25,514.6a136.49,136.49,0,0,0,0,193h0a136.49,136.49,0,0,0,193.05,0L766,383.94a136.45,136.45,0,0,0-96.53-233Z"/><rect x="363.62" y="401.3" width="288.02" height="95.94" transform="translate(466.36 -227.36) rotate(45)" style="fill:#dae0e8"/><path d="M575.54,595.63,361.27,381.36l78.45-78.45L654,517.18ZM382.48,381.36,575.54,574.42l57.24-57.24-193.06-193Z"/><path d="M678.92,761.22A189.27,189.27,0,0,1,677.1,787C664.53,871.57,591.73,936.6,503.55,936.6S342.4,871.57,329.83,787A189.27,189.27,0,0,1,328,761.22a191.78,191.78,0,0,1,1.82-26c12.57-84.54,85.53-149.56,173.72-149.56s161,65,173.55,149.56A191.78,191.78,0,0,1,678.92,761.22Z" style="fill:#f4bd42;fill-rule:evenodd"/><path d="M503.55,944.1a183.21,183.21,0,0,1-181.14-156,192.65,192.65,0,0,1,0-53.91,183.07,183.07,0,0,1,362.12-.08,193.16,193.16,0,0,1,0,53.91,183.07,183.07,0,0,1-181,156.05Zm0-350.92c-82.67,0-154.17,61.55-166.31,143.17a183.88,183.88,0,0,0-1.73,24.87A181.7,181.7,0,0,0,337.26,786c12.12,81.54,83.62,143.09,166.29,143.09s154-61.55,166.14-143.17a178.11,178.11,0,0,0,0-49.67C657.55,654.73,586.12,593.18,503.55,593.18Z"/><path d="M678.92,761.22A189.27,189.27,0,0,1,677.1,787H329.83A189.27,189.27,0,0,1,328,761.22a191.78,191.78,0,0,1,1.82-26H677.1A191.78,191.78,0,0,1,678.92,761.22Z" style="fill:#dae0e8;fill-rule:evenodd"/><path d="M683.65,794.53H323.28l-.88-6.48a192.59,192.59,0,0,1,0-53.83l.88-6.48H683.65l.89,6.48a193.6,193.6,0,0,1,0,53.83Zm-347.17-15h334a176.92,176.92,0,0,0,1-18.31,179.28,179.28,0,0,0-1-18.48h-334a179.28,179.28,0,0,0-1,18.48A177.06,177.06,0,0,0,336.48,779.53Z"/><path d="M855.06,541H827.92V513.82a23.18,23.18,0,0,0-23.18-23.18h0a23.18,23.18,0,0,0-23.17,23.18V541H754.43a23.18,23.18,0,0,0-23.18,23.18h0a23.18,23.18,0,0,0,23.18,23.17h27.14v27.14a23.18,23.18,0,0,0,23.17,23.18h0a23.18,23.18,0,0,0,23.18-23.18V587.31h27.14a23.18,23.18,0,0,0,23.18-23.17h0A23.18,23.18,0,0,0,855.06,541Z" style="fill:#ef4343;fill-rule:evenodd"/><path d="M804.74,645.13a30.71,30.71,0,0,1-30.67-30.68V594.81H754.43a30.68,30.68,0,1,1,0-61.35h19.64V513.82a30.68,30.68,0,0,1,61.35,0v19.64h19.64a30.68,30.68,0,1,1,0,61.35H835.42v19.64A30.71,30.71,0,0,1,804.74,645.13Zm-50.31-96.67a15.68,15.68,0,1,0,0,31.35h34.64v34.64a15.68,15.68,0,1,0,31.35,0V579.81h34.64a15.68,15.68,0,1,0,0-31.35H820.42V513.82a15.68,15.68,0,0,0-31.35,0v34.64Z"/></svg>
              <h3 class="mt-3 h4">Layanan Antar Obat</h3>
              <p>Layanan antar obat sampai ke rumah dengan ama, nyaman dan cepat.</p>

            </router-link>
          </b-col>
        </b-row>
      </b-container>
    </section>

    <section id="contact">
      <b-container class="py-5">
        <b-row>
          <b-col md="6">
            <h3 class="text-montserrat"><em>Medical Checkup</em> Gratis!</h3>
            <p class="text-muted">Jika anda mengalami kendala ketika datang ke kantor kami, anda dapat mengisi formulir berikut untuk membuat jadwal pertemuan dengan dokter kami dan konsultasi dengan tim kami secara gratis.</p>
            <ul class="list-checker">
              <li>Jelaskan apa yang anda keluhkan</li>
              <li>Tim ahli kesehatan kami akan membantu anda</li>
              <li>Membuat resep obat</li>
              <li>Bayar semua tagihan obat dan jasa kami</li>
              <li>Mengirimkan obat dalam waktu 3 jam</li>
              <li>Anda sembuh</li>
            </ul>
          </b-col>
          <b-col md="6">
            <b-card class="border-0 shadow mt-3 mt-md-0">

              <h3>Isi Formulir Dibawah</h3>

              <div class="form-group">
                <div class="form-floating form-floating-alt">
                  <input id="nama" type="text" placeholder="Contoh: Paijo" name="nama" class="form-control" />
                  <label for="nama">Nama Lengkap</label>
                </div>
              </div>

              <div class="form-group">
                <div class="form-floating form-floating-alt">
                  <input id="nomor_hp" type="text" placeholder="Contoh: 085123222121" name="nomor_hp" class="form-control" />
                  <label for="nomor_hp">Nomor HP</label>
                </div>
              </div>

              <div class="form-group">
                <label>Pilihan Tempat Praktek</label>
                <div class="input-card-container column">
                  <label for="ngawi_kota" class="input-custom-card">
                    <input id="ngawi_kota" type="radio" name="pilihan-ganda" class="custom-card">
                    <div class="input-wrap">
                      <div class="input-header">
                        <div class="indicator"></div>
                        Kantor Ngawi Kota
                      </div>
                      <div class="input-body">
                        Jl. Bernadip, No. 12, Ngawi, Jawa Timur
                      </div>
                    </div>
                  </label>
                  <label for="karangjati" class="input-custom-card">
                    <input id="karangjati" type="radio" name="pilihan-ganda" class="custom-card">
                    <div class="input-wrap">
                      <div class="input-header">
                        <div class="indicator"></div>
                        Kantor Karangjati
                      </div>
                      <div class="input-body">
                        Jl. Raya Ngawi-Caruban KM 20, Legundi, Karangjati (Samping Balai Desa Karangjati), No. 12, Ngawi, Jawa Timur
                      </div>
                    </div>
                  </label>
                  <label for="widodaren" class="input-custom-card">
                    <input id="widodaren" type="radio" name="pilihan-ganda" class="custom-card">
                    <div class="input-wrap">
                      <div class="input-header">
                        <div class="indicator"></div>
                        Kantor Widodaren
                      </div>
                      <div class="input-body">
                        Jl. Raya Solo-Ngawi KM 12, Gendingan (Samping Terminal Gendingan) No. 12, Widodaren, Ngawi, Jawa Timur
                      </div>
                    </div>
                  </label>
                </div>
              </div>

              <b-button variant="primary" block class="mt-3">Kirimkan<i class="fas fa-arrow-right ml-2"></i></b-button>

            </b-card>
          </b-col>
        </b-row>
      </b-container>
    </section>

    <Footer />
  </div>
</template>

<script>
import imgHead from '../static/bg-header-home.jpg'
import imgPer from '../static/person.png'

export default {
  name: 'HomePage',
  scrollToTop: true,
  data: () => ({
    imgHeader: imgHead,
    imgHuman: imgPer,

    buttonSm: false,
  }),
  head: {
    title: 'SIRUS - Sistem Informasi Rumah Sakit',
  },
  methods: {
    scrollTo(el) {
      const element = document.getElementById(el);
      element.scrollIntoView({behavior: "smooth", block: "end"});
    }
  },
  mounted() {},
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
  @media screen and (max-width: 600px) {
    padding: .25rem .5rem;
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
    font-weight: 700;
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

#services a.card {
  color: var(--dark);
  text-decoration: none;
  border: 1px solid var(--white) !important;
  transition: all .2s;

  p {
    color: rgb(104, 104, 104);
  }

  &:hover {
    box-shadow: none;
    border-color: rgb(244, 189, 66) !important;
    background: rgb(253, 248, 240);
  }
  &:focus {
    background: rgb(244, 189, 66);
    color: #fff !important;
    p {
      color: rgb(255, 250, 240);
    }
  }
}

#contact {
  .list-checker {
    list-style: none;
    padding: 0;

    li {
      color: #6c757d;
      padding: .35rem 0;

      &::before {
        padding-right: 1rem;
        content: "\f00c";
        font-family: "Font Awesome 5 Free";
        font-size: 14px;
        font-weight: 900;
        line-height: 26px;
        color: #0070cd;
      }
    }
  }
}
</style>
