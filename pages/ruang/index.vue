<template>
    <div class="container">
      <div class="header">
        <img src="smkn4.jpg" alt="Logo" class="logo">
        <h1>Kabeng Toi</h1>
        <p>Jl. Depok, Sukamenak, Purbaratu</p>
        <p>catatan kepala bengkel toi SMKN 4 Tasikmalaya</p>
      </div>
      <div class="content">
        <h2>Peminjaman Barang</h2>
        <div class="form-group">
          <label>Nama Lengkap</label>
          <input type="text" class="form-control" v-model="namaLengkap">
        </div>
        <div class="form-group">
          <label>Jenis Kelamin</label>
          <select class="form-control" v-model="jenisKelamin">
            <option value="">Pilih Jenis Kelamin</option>
            <option value="Laki-laki">Laki-laki</option>
            <option value="Perempuan">Perempuan</option>
          </select>
        </div>
        <div class="form-group">
          <label>Tanggal Lahir</label>
          <input type="date" class="form-control" v-model="tanggalLahir">
        </div>
        <div class="form-group">
          <label>Alamat</label>
          <textarea class="form-control" v-model="alamat"></textarea>
        </div>
        <button class="btn btn-primary" @click="submitForm">Simpan</button>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        namaLengkap: '',
        jenisKelamin: '',
        tanggalLahir: '',
        alamat: ''
      }
    },
    methods: {
      submitForm() {
        // kode untuk mengirimkan data ke server
        console.log('Data telah dikirimkan ke server')
      }
    }
  }
  </script>
  
  <style scoped>
  .container {
    max-width: 800px;
    margin: 40px auto;
    padding: 20px;
    background-color: #f9f9f9;
    border: 1px solid #ddd;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  }
  
  .header {
    display: flex;
    align-items: center;
    margin-bottom: 20px;
  }
  
  .logo {
    width: 50px;
    height: 50px;
    margin-right: 10px;
  }
  
  h1 {
    font-size: 24px;
    font-weight: bold;
    margin-bottom: 10px;
  }
  
  p {
    font-size: 18px;
    color: #666;
  }
  
  .content {
    margin-top: 20px;
  }
  
  .form-group {
    margin-bottom: 20px;
  }
  
  label {
    display: block;
    margin-bottom: 10px;
  }
  
  input[type="text"], input[type="date"], select, textarea {
    width: 100%;
    height: 40px;
    padding: 10px;
    margin-bottom: 20px;
    border: 1px solid #ccc;
  }
  
  button[type="submit"] {
    background-color: #4CAF50;
    color: #fff;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
  }
  
  button[type="submit"]:hover {
    background-color: #3e8e41;
  }
  </style>