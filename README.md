# Struktur Antar Hubungan

Nama: Ahmad Fatik Aji Bagaskara
Nim: 09011382429176
Kelas: SKU2B

### 1. **Struktur Antar Hubungan dan Contohnya**

Struktur antar hubungan itu kayak cara komponen-komponen dalam komputer "ngobrol" satu sama lain. Bayangin aja, komputer itu kayak tim kerja. CPU, memori, dan perangkat I/O itu anggotanya. Nah, biar mereka bisa kerja bareng, harus ada cara buat mereka berkomunikasi. Itulah yang disebut struktur antar hubungan.

**Contohnya:**
- **Bus System**: Ini kayak jalan raya buat data. CPU, memori, dan perangkat I/O terhubung ke satu jalur yang sama buat ngirim dan nerima data. Misalnya, waktu CPU mau ngambil data dari memori, data itu lewat bus. Tapi, karena jalurnya cuma satu, kadang bisa macet kalo terlalu banyak yang mau lewat.

  **Contoh Nyata**: Bayangin bus kayak jalan tol. CPU itu mobil yang mau ke memori (rumah). Bus data itu jalannya, bus alamat itu petanya. Kalo jalan tolnya rame, ya pasti lama sampe rumahnya.

- **Point-to-Point**: Ini kayak jalur khusus. Setiap komponen punya jalur sendiri buat ngobrol sama komponen lain. Jadi, nggak perlu lewat jalan umum.

  **Contoh Nyata**: Kayak chat pribadi di WhatsApp. Cuma dua orang yang ngobrol, nggak perlu lewat grup yang rame.

- **Crossbar Switch**: Ini lebih canggih lagi. Kayak jaringan telepon jaman dulu, di mana setiap telepon bisa terhubung ke telepon lain lewat operator.

  **Contoh Nyata**: Bayangin lagi pesta. Hostnya ngatur siapa yang boleh ngobrol sama siapa. Jadi, nggak semua orang ngobrol bareng-bareng.

---

### 2. **Kenapa Kinerja Bisa Turun Kalo Terlalu Banyak Perangkat Terhubung ke Bus?**

Bayangin bus itu kayak jalan tol. Kalo terlalu banyak mobil (perangkat) yang mau lewat, pasti macet. Nah, ini beberapa penyebabnya:

- **Lalu Lintas Padat**: Kalo semua perangkat mau ngirim data barengan, bus jadi penuh. Akibatnya, data harus ngantri buat lewat. Ini bikin prosesnya jadi lama.

- **Konflik Akses**: Semua perangkat harus berebut buat pake bus. Kalo banyak yang mau pake, ya pasti ada yang harus nunggu.

- **Bandwidth Terbagi**: Bandwidth itu kayak lebar jalan tol. Kalo terlalu banyak mobil, jalan tolnya jadi sempit buat masing-masing mobil. Akibatnya, data nggak bisa jalan cepat.

- **Latensi Tinggi**: Latensi itu waktu yang dibutuhin buat data sampe ke tujuan. Kalo bus rame, data harus nunggu lama buat bisa jalan.

**Contoh Nyata**: Bayangin lagi jalan tol. Kalo cuma ada 5 mobil, lancar jaya. Tapi kalo ada 50 mobil, ya pasti macet. Mobil-mobil itu harus ngantri buat lewat, dan sampe tujuan jadi lama.

---

### 3. **Kenapa Perangkat Prioritas 16 Bisa Punya Waktu Tunggu Paling Cepat?**

Biasanya, perangkat prioritas tinggi kayak CPU selalu dilayani lebih dulu. Tapi, ada kalanya perangkat prioritas rendah (kayak prioritas 16) malah punya waktu tunggu lebih cepat. Kok bisa?

- **Jarang Minta Akses**: Perangkat prioritas rendah biasanya nggak sering minta akses ke bus atau CPU. Karena jarang minta, pas mereka minta, nggak perlu nunggu lama.

- **Waktu Senggang**: Kalo perangkat prioritas tinggi lagi nggak sibuk, perangkat prioritas rendah bisa "nyelinap" dan dapet akses lebih cepat.

- **Manajemen Sistem yang Baik**: Sistem yang cerdas bisa ngatur waktu akses dengan baik, jadi perangkat prioritas rendah nggak perlu nunggu lama.

**Tapi, Ini Nggak Selalu Berlaku**:
- **Kalo Perangkat Prioritas Rendah Jadi Sibuk**: Misalnya, tiba-tiba perangkat prioritas rendah mulai minta akses lebih sering. Nah, waktu tunggunya bakal naik karena mereka harus ngantri sama perangkat lain.

- **Sistem yang Nggak Efisien**: Kalo sistemnya nggak ngatur prioritas dengan baik, perangkat prioritas rendah bisa aja tetep nunggu lama meskipun jarang minta akses.

**Contoh Nyata**: Bayangin lagi restoran cepat saji. Pelanggan VIP selalu dilayani lebih dulu. Tapi kalo nggak ada VIP, pelanggan biasa bisa langsung dilayani tanpa nunggu. Tapi, kalo tiba-tiba banyak pelanggan biasa datang, ya mereka harus ngantri juga.

---

Jadi, gitu penjelasannya! Semoga lebih mudah dipahami ya. Kalo masih ada yang bingung, tanya aja! 😄
