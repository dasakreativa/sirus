<template>
  <div :class="responsive == true ? 'table-responsive' : ''">
    <b-row>
      <b-col>
        <label for="filter">Tampilkan Per</label>
        <b-form-select v-model="selected" :options="options" />
      </b-col>
      <b-col>
        <div class="form-group">
          <label for="filter">Cari</label>
          <input type="text" id="filter" placeholder="Cari sesuatu..." v-model="filter" class="form-control" />
        </div>
      </b-col>
    </b-row>

    <b-table striped hover show-empty :fields="fields" :filter="filter" :per-page="selected" :current-page="currentPage" :items="data">
      <template #cell(status)="data">
        <span class="badge badge-success" v-if="data.item.terisi / data.item.jumlah <= 0.25">Longgar</span>
        <span class="badge badge-warning" v-else-if="data.item.terisi / data.item.jumlah <= 0.5">Agak Longgar</span>
        <span class="badge badge-danger" v-else-if="data.item.terisi / data.item.jumlah < 1">Agak Penuh</span>
        <span class="badge badge-dark" v-else-if="data.item.terisi / data.item.jumlah == 1">Penuh / Kosong</span>
      </template>
    </b-table>

    <b-row class="mt-3">
      <b-col>&nbsp;</b-col>
      <b-col>
        <b-pagination class="justify-content-end" v-model="currentPage" :total-rows="rows" :per-page="selected" />
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {
  props: ["data", "responsive"],
  data: () => ({
    filter: "",

    currentPage: 1,
    selected: "10",
    options: [
      { value: null, text: 'Pilih Satu' },
      { value: 10, text: '10 Per Halaman' },
      { value: 20, text: '20 Per Halaman' },
      { value: 30, text: '30 Per Halaman' },
      { value: 50, text: '50 Per Halaman' },
      { value: 100, text: '100 Per Halaman' },
      { value: 500, text: '500 Per Halaman' },
    ],

    fields: [
      {
        key: 'daerah',
        sortable: true,
        label: 'Wilayah Cakupan',
      },
      {
        key: 'puskesmas',
        sortable: true,
        label: 'Puskesmas/Rumah Sakit',
      },
      {
        key: 'jumlah',
        label: 'Jumlah Kamar',
        sortable: true,
      },
      {
        key: 'terisi',
        sortable: true,
        label: 'Jumlah Kamar Yang Terisi',
      },
      {
        key: 'status',
        sortable: false,
        label: 'Status',
      },
    ],
  }),
  computed: {
    rows() {
      return this.data.length;
    }
  }
}
</script>
