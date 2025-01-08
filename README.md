Berikut adalah panduan langkah-langkah untuk mengatur TailwindCSS dengan format yang terstruktur:

---

## **Mengatur TailwindCSS**

1. **Buka Visual Studio Code (VS Code)**  
2. **Buka Terminal di VS Code**  
3. **Membuat Folder untuk Proyek**  
   ```bash
   $ mkdir tailwindcss
   ```
4. **Masuk ke Folder TailwindCSS**  
   ```bash
   $ cd tailwindcss
   ```
5. **Inisialisasi Proyek dengan NPM**  
   ```bash
   $ npm init -y
   ```
6. **Install TailwindCSS dan Dependencies**  
   ```bash
   $ npm install tailwindcss autoprefixer postcss -D
   ```
7. **Inisialisasi File Konfigurasi TailwindCSS**  
   ```bash
   $ npx tailwindcss init
   ```
8. **Buat Folder "src" di dalam Folder TailwindCSS**  
9. **Buat File `global.css` di Dalam Folder "src"**  
10. **Masukkan Kode Berikut ke Dalam `global.css`**  
    ```css
    @tailwind base;
    @tailwind components;
    @tailwind utilities;
    ```
11. **Masukkan Kode Berikut ke Dalam `tailwind.config.js`**  
    ```javascript
    /** @type {import('tailwindcss').Config} */
    module.exports = {
      content: ["./src/**/*.{html,js}", "../*.{html,js}"],
      theme: {
        extend: {},
      },
      plugins: [],
    }
    ```
12. **Buat File `index.html` di Luar Folder TailwindCSS**  
13. **Tambahkan Kode Berikut ke Dalam `<head>` File `index.html`**  
    ```html
    <link rel="stylesheet" href="tailwindcss/src/global-output.css">
    ```
14. **Tambahkan Kode Berikut ke Dalam `package.json`**  
    ```json
    "scripts": {
      "test": "echo \"Error: no test specified\" && exit 1",
      "tailwind:watch": "npx tailwindcss -i ./src/global.css -o ./src/global-output.css --watch"
    }
    ```
15. **Jalankan TailwindCSS**  
    - Pastikan terminal berada di folder `tailwindcss`.  
    - Jalankan perintah berikut untuk memulai TailwindCSS dalam mode pemantauan:  
      ```bash
      $ npm run tailwind:watch
      ```
16. **Selesai** 🎉

---

Dengan format ini, langkah-langkahnya menjadi lebih terstruktur dan mudah diikuti. Jika ada bagian yang perlu disesuaikan, beri tahu saya! 😊
