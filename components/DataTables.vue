<template>
  <div :class="responsive == true ? 'table-responsive' : ''">
    <b-row class="align-items-end">
      <b-col>
        <div class="form-group">
          <label for="filter">Tampilkan Per</label>
          <b-form-select v-model="selected" :options="options" />
        </div>
      </b-col>
      <b-col>
        <div class="form-group d-inline floating">
          <div class="form-floating m-0 pb-3">
            <input id="filter" v-model="filter" type="text" placeholder="Cari sesuatu..." class="form-control" />
            <label for="filter">Cari Data</label>
          </div>
        </div>
      </b-col>
    </b-row>

    <b-table striped responsive hover show-empty :fields="fields" :filter="filter" :per-page="selected" :current-page="currentPage" :items="data">
      <template #cell(status)="items">
        <span v-if="items.item.terisi / items.item.jumlah <= 0.25" class="badge badge-success">Longgar</span>
        <span v-else-if="items.item.terisi / items.item.jumlah <= 0.5" class="badge badge-warning">Agak Longgar</span>
        <span v-else-if="items.item.terisi / items.item.jumlah < 1" class="badge badge-danger">Agak Penuh</span>
        <span v-else-if="items.item.terisi / items.item.jumlah == 1" class="badge badge-dark">Penuh / Kosong</span>
      </template>
    </b-table>

    <b-row class="mt-3">
      <b-col>&nbsp;</b-col>
      <b-col>
        <b-pagination v-model="currentPage" class="justify-content-end" :total-rows="rows" :per-page="selected" />
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
  },
  methods: {
  },
}
</script>
