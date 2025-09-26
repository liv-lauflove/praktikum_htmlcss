Penjelasan HTML dan CSS

Nama: Olyvia Audy Djohari  
NIM: 42430058  

PRAKTIKUM MEMBUAT CURRICULUM VITAE HTML DAN CSS  

Penjelasan kode html:  
1. Struktur dokumen html
<img width="619" height="183" alt="image" src="https://github.com/user-attachments/assets/38a6eb9a-9cd8-4d5c-8fd3-91c1a045a389" />

`<!DOCTYPE html>` untuk mendefinisikan bahwa dokumen ini adalah HTML 

`<html lang="en">` adalah tag utama yang membungkus semua isi, dengan bahasa Inggris.  

`<head>` berisi informasi metadata seperti charset, viewport (biar responsif), title, dan link ke file CSS eksternal.  

`<body>` berisi seluruh konten yang akan ditampilkan di halaman web.  

---

2. Navigasi
<img width="548" height="216" alt="image" src="https://github.com/user-attachments/assets/59f9229f-5886-40c2-aa8e-e3113afe84ef" />
Bagian ini berisi menu navigasi berbentuk unordered list (`<ul>` dengan `<li>`).  
Setiap item pakai `<a href="#idsection">` untuk menghubungkan ke bagian tertentu di halaman (scroll ke section terkait).  
Terdapat 5 menu yaitu, About Me, Education, Hobbies, Skills, Contact Me.  

---

3. Header
<img width="699" height="164" alt="image" src="https://github.com/user-attachments/assets/daed5095-c044-434b-b6e3-90bc3308ca56" /
Berfungsi menampilkan informasi profil utama.  
Ada foto (`<img>`), nama lengkap (`<h1>`), teks paragraf (`<p>`), dan emoji.  

---

4. Main content 
Menggunakan semantic html yaitu section untuk membagi bagian-bagian penting, disetiap section menambahkan <br> untuk enter dan berikan space, ada 5 section:  

- Section About Me (`<section id="aboutme">`)
  <img width="892" height="319" alt="image" src="https://github.com/user-attachments/assets/2140d972-db10-4907-8797-538bc3f59a97" />
Berisi teks perkenalan diri, yaitu nama, latar belakang pendidikan. Menambah gambar coding dengan tag `<img>`.  

- Section Education (`<section id="education">`)
  <img width="463" height="187" alt="image" src="https://github.com/user-attachments/assets/17765eab-8ae9-4ff3-9910-5fbb6c0304e5" />
  Menyimpan daftar riwayat pendidikan dengan tag `<ul>` (SD, SMP, SMA).  
  Ditampilkan berurutan sebagai list

- Section Hobbies (`<section id="hobbies">`)
  <img width="551" height="682" alt="image" src="https://github.com/user-attachments/assets/db832a4c-af9c-4a2e-8dbb-3fb3365a8459" />
  Menampilkan daftar hobi, setiap hobi ada teks deskripsi (`<p>`) + gambar (`<img>`).  
  Membuat class hobbybox pada setiap hobby agar bisa membuat tampilan kotak per hobi.  

- Section Skills (`<section id="skills">`)
  <img width="390" height="407" alt="image" src="https://github.com/user-attachments/assets/6dc303ca-b9c0-45a6-a300-0750babdcc8a" />
  Dibuat dengan container berisi beberapa skill card. Setiap card punya judul (`<h3>`) dan isi (`<p>`).  

- Section Contact Me (`<section id="contactme">`)
  <img width="739" height="219" alt="image" src="https://github.com/user-attachments/assets/b6596b9e-2e01-4aae-b76b-ba26319fa62d" />
  Berisi kontak untuk dihubungi, terdapat teks paragraf singkat + daftar kontak (`<ul>`).  
  Membuat list dengan link yang mengarahkan ke kontak.

setelah itu ditutup dengan tag </main>, </body>, dan </html>

---

 CSS:  

1. body
   <img width="308" height="91" alt="image" src="https://github.com/user-attachments/assets/50b6c562-5725-4f26-938e-9f4e3016afcb" />
- `margin: 0px;` untuk menghilangkan jarak default browser.  
- `background-color: #c8d9e6;` untuk memberi warna biru muda ke seluruh halaman.  

2. header
   <img width="712" height="656" alt="image" src="https://github.com/user-attachments/assets/cbbee947-3708-4851-8058-32c253c7e74d" />
  #header
- `display: flex;` untuk membuat header menggunakan flexbox.  
- `align-items: center;` menjajarkan foto & teks di tengah secara vertikal.  
- `gap: 20px;` untuk memberi jarak antara foto dan teks.  
- `justify-content: center;` untuk memposisikan semua isi ke tengah halaman.  
- `padding: 20px;` untuk memberi ruang dalam.  
- `border-radius: 8px;` untuk sudut melengkung.  
- `margin: 30px;` untuk memberi jarak luar dari tepi halaman.  
- `background-color: #f7f2eb;` untuk warna krem pada header.  

#header img
- `width/height: 150px;` ukuran foto kotak.  
- `object-fit: cover;` agar foto proporsional.  
- `border-radius: 50%;` membuat foto bulat.  
- `border: 3px solid #081f5c;` bingkai biru gelap.  

#header .info
- `display: flex; flex-direction: column;` untuk teks ditata vertikal.  
- `line-height: 1.6;` beri jarak antar baris  

#header h1  
- `margin: 0;` hilangkan jarak default judul.  
- `font-size: 28px;` ukuran besar untuk nama.  
- `color: #081f5c;` beri warna biru gelap untuk tulisan  

#header p  
- `margin: 0;` hilangkan jarak default paragraf.  
- `font-size: 18px;` ukuran sedang.  
- `color: #081f5c;` beri warna biru gelap untuk tulisan 

3. main
   <img width="193" height="84" alt="image" src="https://github.com/user-attachments/assets/789f6a4a-69f4-4bc9-9e9a-b5f484471709" />

- `margin: 20px;` memberi jarak luar untuk konten utama agar tidak menempel ke tepi layar.  

4. navigasi
   <img width="519" height="407" alt="image" src="https://github.com/user-attachments/assets/af1d875e-9c8c-4686-9e7f-f9c9a44bf6a4" />
navbar ul 
- `list-style: none;` hilangkan bullet list.  
- `display: flex; justify-content: flex-end;` atur menu jadi horizontal dan rata kanan.  
- `background-color: #081F5C;` beri warna biru tua.  

navbar a
- `color: #fff9f0;` teks putih krem.  
- `text-decoration: none;` hilangkan garis bawah.  
- `padding: 15px;` beri ruang agar terlihat seperti tombol.  
- `font-weight: bold;` teks tebal.  

navbar a:hover  
- `background-color: #0b3d91;` saat hover, latar belakang link berubah biru lebih terang, memberi efek interaktif.  

---

5. About me
   <img width="730" height="698" alt="image" src="https://github.com/user-attachments/assets/ecbecb9b-007d-47f0-8cef-c4a0b0c009f4" />
- Semua section diberi border.  
- `.aboutcontainer { display: flex; }` teks dan gambar sejajar horizontal.  
- `justify-content: space-between;` teks di kiri, gambar di kanan.  
- `align-items: center;` rata tengah vertikal.  
- `gap: 30px;` jarak antar teks dan gambar.  
- `max-width: 600px;` batasi lebar teks.  
- `object-fit: cover;` gambar proporsional.  
- `border-radius: 10px;` sudut gambar melengkung.  

6. Education
   <img width="586" height="657" alt="image" src="https://github.com/user-attachments/assets/450048a3-ecde-4cb0-a90d-871591ecff9c" />
   sebagian besar sudah dijelaskan sebelumnya, kecuali:
- transform: translateY(-3px); ini CSS untuk menggeser elemen secara vertikal.
translateY berarti geser di sumbu Y (atas-bawah).
Angka -3px artinya elemen digeser sedikit ke atas saat di-hover.

7. Hobby
   <img width="590" height="711" alt="image" src="https://github.com/user-attachments/assets/9e44a19a-18a9-4d19-a987-2edf2652e3f9" />
- display: grid; membuat layout kotak hobi pakai CSS Grid, lebih fleksibel untuk membagi kolom/baris.
grid-template-columns: repeat(auto-fit, minmax(180px, 1fr)); ngatur jumlah kolom otomatis
- auto-fit jumlah kolom menyesuaikan ukuran layar. minmax(180px, 1fr) tiap kolom minimal 180px, maksimal bisa melebar sampai membagi ruang sama rata (1fr).
Hasilnya: kotak hobi bisa responsif, tetap rapi di layar kecil maupun besar.
- object-fit: cover; bikin gambar di dalam img tetap penuh menutupi box, tanpa ketarik/distorsi, meski dipotong.
- transition: transform 0.2s ease, background-color 0.2s ease; bikin animasi halus saat hover: transform (geser naik turun) dan background-color (warna latar) berubah pelan (0.2 detik).
 

8 Skills
  <img width="484" height="784" alt="image" src="https://github.com/user-attachments/assets/c4cfaba9-1703-47d6-a7f0-2a4fcc803c1a" />
-Memberikan background color, dan padding/jarak dalam dari isi elemen ke tepi yaitu 40 pixel, memerikan jarak luar elemen dari elemen lain/margin, membuat sudut elemen melengkung atau border radius. box-shadow: 0 2px 6px rgba(0,0,0,0.1); untuk membuat bayangan di sekitar elemen, mengatur teks menjadi rata tengah dan ukuran font 18px. 
- `#skills h2` diberi warna teks dan margin-bottom.  
- Kontainer yang berisi .skillscontainer {
    display: flex;  menggunakan Flexbox untuk tata letak 
    justify-content: space-around; memberi jarak sama antar elemen 
    flex-wrap: wrap; membungkus elemen ke baris baru jika perlu 
    gap: 20px; jarak antar elemen flex
} 
- Class skillcard=
box-shadow: 0 2px 6px rgba(0,0,0,0.1); untuk buat bayangan lembut 
transition: transform 0.2s ease-in-out; buat efek transisi saat hover 
pseudo-class selector :hover = transform: translateY(-5px); untuk menggerakkan elemen secara vertical ke atas sebesar 5 pixel pada saat hover.
Memberikan warna teks dan margin bottom pada h3 kelas skillcard serta menambahkan warna teks, ukuran teks, jarak antar baris ke teks paragraph . 


9. Contact me
    <img width="517" height="769" alt="image" src="https://github.com/user-attachments/assets/36fcfe48-4bb4-45f3-ab1e-d370376c0e5d" />
- memberikan background-color, warna teks, padding 40px, margin 50px auto, border-radius 10px, box-shadow, max-width 600px, text-align center, font-size 18px.  
- `#contactme h2` warna teks dan margin bawah 20px.  
- `#contactme p` margin bawah 15px, font-size 18px, warna.  
- `#contactme ul` tanpa bullet dan padding.  
- `#contactme li` margin 10px atas-bawah, font-size 18px.  
- `#contactme a` warna, tanpa garis bawah, tebal, transisi warna.  
- `#contactme a:hover` warna berubah #ffe1e6 dan underline.  
- `@media screen and (max-width: 600px)` adlaah media query untuk desain responsif, mengatur elemen main agar lebarnya menjadi 100px jika layar berukuran 600px atau lebih kecil.

  
