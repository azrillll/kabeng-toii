<template>
    <div class="container">
      <h1>Buat akun</h1>
      <div class="input-group">
        <label for="username">USERNAME</label>
        <input type="text" id="username" placeholder="Masukkan username">
      </div>
      <div class="input-group">
        <label for="password">PASSWORD</label>
        <input type="password" id="password" placeholder="Masukkan password">
      </div>
      <div class="button-group">
        <button class="button" @click="keluar">Keluar</button>
        <button class="button" @click="buatAkun">Buat</button>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    methods: {
      keluar() {
        // Implementasikan logika keluar dari halaman
      },
      buatAkun() {
        // Implementasikan logika pembuatan akun
      }
    }
  }
  </script>
  
  <style scoped>
  .container {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 100vh;
    width: 100%;
    background-color: #f4f4f4;
  }
  
  h1 {
    font-size: 2rem;
    margin-bottom: 2rem;
  }
  
  .input-group {
    display: flex;
    flex-direction: column;
    margin-bottom: 1rem;
  }
  
  .input-group label {
    font-weight: bold;
    margin-bottom: 0.5rem;
  }
  
  .input-group input {
    padding: 1rem;
    border: 1px solid #ccc;
    border-radius: 4px;
  }
  
  .button-group {
    display: flex;
    gap: 1rem;
  }
  </style>
