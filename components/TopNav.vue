<template>
  <div id="navtop">
    <b-navbar toggleable="md" :type="navbarType" :class="navbarFx == 'top' ? 'shadow' : ''" :fixed="navbarFx" :variant="navbarBg">
      <b-container>
        <b-navbar-brand to="/"><img :src="img" alt="Logo Sirus" height="35px" class="mr-2" /></b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav class="ml-auto">
            <b-nav-item to="/cek-oksigen">Stok Oksigen</b-nav-item>
            <b-nav-item to="/cek-ranap">Kamar Ranap</b-nav-item>
            <b-nav-item to="/cek-vaksinasi">Data Vaksinasi</b-nav-item>
          </b-navbar-nav>

          <b-button variant="primary" @click="$bvModal.show('modal-login')"><i class="fas fa-sign-in-alt mr-2"></i>Masuk</b-button>
        </b-collapse>
      </b-container>
    </b-navbar>

    <b-modal id="modal-login" title="Maaf!">
      <p>Maaf, untuk situs hanya sampai sini saja. Kami akan mengembangkan situs ini lebih lanjut kedepannya.</p>
    </b-modal>
  </div>
</template>

<script>
import imgsLight from '../static/brands/logo-color-alt.svg'
import imgsDark from '../static/brands/logo-white-alt.svg'

export default {
  name: 'Navbar',
  data() {
    return {
      img: imgsLight,

      navbarType: 'light',
      navbarBg: 'transparent',
      navbarFx: '',
    }
  },
  mounted() {
    window.document.onscroll = () => {
      if(window.scrollY > 200) {
        this.navbarType = 'dark';
        this.navbarBg = 'primary';
        this.navbarFx = 'top';

        this.img = imgsDark;
      } else {
        this.navbarType = 'light';
        this.navbarBg = 'transparent';
        this.navbarFx = '';

        this.img = imgsLight;
      }
    };
  }
}
</script>
