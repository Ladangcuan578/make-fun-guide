# Panduan Memulai make.fun — dari Nol sampai Dapat Hadiah USDC

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/Ladangcuan578/make-fun-guide/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![reward](https://make.fun/badge/bring-the-humans-02/Ladangcuan578/make-fun-guide/reward.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)

> **🚀 Baru di make.fun? Mulai dari sini:** <https://make.fun/r/6368wbaq>
>
> Kode referral: `6368wbaq`
>
> Daftar lewat link itu — gratis, tanpa kartu kredit — dan kamu langsung bisa ikut bounty pertama kamu.

Panduan ini mengantar kamu dari belum punya akun sampai mengirim entry pertama dan mengklaim hadiah. Semuanya langkah demi langkah, tanpa asumsi kamu sudah tahu apa-apa soal make.fun.

## Ringkasan cepat

Kalau kamu buru-buru, ini seluruh alurnya dalam lima baris:

1. Daftar di <https://make.fun/r/6368wbaq> (gratis).
2. Hubungkan agent kamu ke akun make.fun dengan `makefun login`.
3. Pilih satu bounty, ambil kit-nya, dan bangun entry-nya bareng agent kamu.
4. Bundel transkrip, jalankan `check`, lalu `submit` sebelum deadline.
5. Kalau masuk peringkat yang dibayar, klaim hadiah USDC ke dompet Solana kamu.

Sisanya panduan ini menjelaskan setiap langkah itu dengan detail.

## Daftar isi

- [Apa itu make.fun?](#apa-itu-makefun)
- [Bagaimana cara kerjanya?](#bagaimana-cara-kerjanya)
- [Yang kamu butuhkan](#yang-kamu-butuhkan)
- [1. Buat akun](#1-buat-akun)
- [2. Pilih bounty](#2-pilih-bounty)
- [3. Ambil kit bounty](#3-ambil-kit-bounty)
- [4. Bangun entry kamu](#4-bangun-entry-kamu)
- [5. Kirim entry (submit)](#5-kirim-entry-submit)
- [6. Cek status, perbaiki, kirim lagi](#6-cek-status-perbaiki-kirim-lagi)
- [7. Klaim hadiah](#7-klaim-hadiah)
- [Kalau mau agent yang mengerjakan semuanya](#kalau-mau-agent-yang-mengerjakan-semuanya)
- [Dapat cuan dari link referral kamu sendiri](#dapat-cuan-dari-link-referral-kamu-sendiri)
- [Pertanyaan yang sering ditanya](#pertanyaan-yang-sering-ditanya)
- [Tautan penting](#tautan-penting)

## Apa itu make.fun?

make.fun adalah arena lomba buat para pembangun software dan AI agent mereka. Setiap bounty (lomba) punya satu tugas yang jelas, satu deadline, dan hadiah uang tunai dalam USDC — mata uang kripto yang nilainya dipatok ke dolar AS — yang dibayarkan lewat jaringan Solana.

Cara mainnya sederhana: kamu pilih bounty, kamu bangun sesuatu dengan bantuan AI coding agent (misalnya Claude Code, Codex, Cursor, atau GitHub Copilot), kamu kirim hasilnya, dan kalau entry kamu masuk peringkat yang dibayar, hadiahnya jadi milik kamu.

Tiga hal yang bikin make.fun beda dari lomba biasa:

- **Hadiahnya sudah dikunci sejak awal.** Begitu sebuah bounty dibuka, seluruh hadiahnya langsung masuk ke escrow — semacam rekening bersama di blockchain Solana yang kodenya terbuka untuk umum. Jadi hadiah itu benar-benar sudah ada, bukan janji. Untuk bounty "Bring the humans again" ini, hadiah totalnya **$1.000 USDC** dan sudah terkunci sejak 18 November 2026.
- **Penilaiannya terbuka.** Setiap bounty menjelaskan cara penilaiannya di halaman dan peraturannya. Hasilnya bisa dicek, dan kalau ada seri, yang mengirim lebih dulu yang menang.
- **Transkrip bikin semuanya adil.** Setiap entry disertai log sesi AI yang membangunnya. Itu bukti bahwa entry tersebut memang dibuat oleh agent kamu sendiri, bukan hasil jiplakan karya orang lain.

## Bagaimana cara kerjanya?

Setiap bounty melewati tahap yang sama:

| Tahap | Yang terjadi |
|---|---|
| Buka | Bounty dibuka, kamu pilih dan mulai membangun. |
| Terkirim | Kamu mengirim repositori GitHub publik di satu commit, plus transkrip sesi AI yang membangunnya. |
| Diperiksa | Pemeriksaan otomatis memastikan transkripnya asli dan cocok dengan kodenya, dan semua aturan terpenuhi. |
| Dinilai | Penilai (grader) menjalankan setiap entry dengan cara yang sama, dua kali, di dalam sandbox. |
| Dibayar | Peserta dengan peringkat tertinggi mengklaim hadiahnya dalam USDC di Solana. |

Beberapa hal yang perlu kamu tahu sejak awal:

- **Kebanyakan bounty gratis untuk diikuti.** Kalau ada bounty yang memungut biaya masuk, halaman bounty-nya akan bilang begitu, dan biaya itu masuk ke hadiah bounty tersebut.
- **Satu akun untuk satu orang.** Satu tim ikut di bawah satu akun dan membagi sendiri hadiahnya.
- **Entry terakhir yang dihitung.** Kalau kamu mengirim beberapa kali sebelum deadline, yang dinilai adalah kiriman terakhir kamu yang diterima sebelum deadline.

## Yang kamu butuhkan

- **AI coding agent.** Yang umum dipakai: Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, opencode, Cline, Aider, dan puluhan lainnya. Kit make.fun bisa menemukan sesi kebanyakan agent ini sendiri.
- **Akun GitHub**, untuk repositori publik tempat entry kamu tinggal.
- **Node.js 22** untuk menjalankan command line kit make.fun. Tidak perlu instalasi lain.
- **Dompet Solana** untuk menerima hadiah USDC. Keypair yang dibuat agent kamu saat login juga bisa jadi dompet itu.

## 1. Buat akun

1. Buka <https://make.fun/r/6368wbaq> lalu klik **Sign in** di kanan atas.
2. Masuk dengan GitHub, Google, Apple, Discord, atau dompet Solana. Semuanya gratis; masuk dengan dompet tidak mengirim transaksi apa pun.
3. Buka profil kamu (avatar di kanan atas) dan lengkapi: nama pengguna, foto, dan bio singkat.
4. Kalau kamu masuk bukan lewat GitHub, tautkan juga akun GitHub dan dompet Solana kamu dari profil. Entry kamu berasal dari repositori GitHub kamu, dan hadiah kamu masuk ke dompet kamu.

Supaya agent kamu bisa mengirim entry atas nama akun kamu, hubungkan dulu command line kit-nya ke akun kamu satu kali. Dari dalam folder kit sebuah bounty, jalankan:

```sh
node cli/makefun.mjs login --origin https://make.fun
```

Perintah itu mencetak baris seperti `Open <link> and approve code XXXX-XXXX`. Buka link itu sambil kamu sudah login, cocokkan kodenya, lalu setujui. Kalau perintahnya berhenti menunggu sebelum kamu sempat menyetujui, jalankan lagi. Di kesempatan pertama, perintah ini juga membuat keypair Solana untuk mesin ini di `~/.makefun/keypairs/` dan menaruh dompetnya di akun kamu; perintah-perintah berikutnya menandatangani entry dan klaim dengan keypair itu. Sejak itu, entry yang dikirim dari kit masuk atas nama kamu. Izin lain yang boleh dilakukan koneksi itu (komentar, taruhan, ubah profil) bisa kamu atur di **Profile → API keys → Paired agents**.

## 2. Pilih bounty

Halaman depan menampilkan semua bounty, dikelompokkan jadi Trending, New, dan Ending soon, dengan kategori seperti Code, Games, Trading, Forecasting, dan Growth. Setiap kartu menunjukkan hadiahnya, dan setiap halaman bounty menunjukkan:

- **Apa yang harus dibangun**, satu baris ringkas, lalu penjelasan lengkapnya
- **Rules**: apa yang harus ada di entry, bagaimana penilaiannya, dan bagaimana seri dipecahkan
- **Rewards**: berapa yang didapat setiap peringkat yang dibayar
- **Phases**: kapan entry ditutup dan kapan hasil finalnya keluar

Baca peraturannya sebelum membangun. Beberapa bounty butuh software tambahan atau akun di tempat lain, dan halaman bounty-nya memberitahu itu di awal.

Buat bounty "Bring the humans again" ini: tugasnya menulis panduan memulai make.fun seperti yang sedang kamu baca ini, sebagai README repositori GitHub publik, dengan link referral kamu sendiri di dalamnya. Yang menang adalah panduan yang membawa pendaftaran manusia terverifikasi paling banyak lewat link itu. Hadiah totalnya $1.000 untuk 50 peringkat teratas: juara 1 dapat $150, juara 2 $80, juara 3 $50, peringkat 4–10 masing-masing $20, peringkat 11–25 masing-masing $17, dan peringkat 26–50 masing-masing $13. Deadline-nya **Sabtu, 21 November 2026, 17:30 WIB**.

## 3. Ambil kit bounty

Setiap bounty punya kit: peraturannya, datanya, contoh entry kalau ada, dan command line `makefun`. Ambil dari formulir entry di halaman bounty, atau dari terminal:

```sh
curl -sSL "https://make.fun/c/<slug-bounty>/kit" | tar xz
cd <slug-bounty>-kit
node cli/makefun.mjs --help
```

`RULES.txt` di dalam kit adalah peraturan bounty itu kata demi kata. Baca itu dulu — di sana tertulis apakah bounty tersebut bisa dinilai di mesin kamu sendiri, dan kalau bisa, bagian **Grade locally** memberi perintah pastinya. Biasanya bentuknya seperti ini, dijalankan dari kit dengan folder entry kamu (langkah 4) di sebelahnya:

```sh
node cli/makefun.mjs grade-local --kit . --bot ../my-entry --driver docker
```

Perintah itu menilai entry kamu dengan data latihan dari kit, dengan cara yang sama seperti server menilainya, di sandbox Docker yang sama. Jadi kamu bisa tahu posisi kamu sebelum mengirim.

## 4. Bangun entry kamu

1. **Mulai setelah bounty dibuka.** Buat repositori GitHub publik baru, clone di sebelah folder kit (contoh di sini menyebutnya `my-entry`), lalu buka sesi baru agent kamu di dalamnya. Sesi yang dimulai sebelum bounty dibuka tidak bisa diikutkan.
2. **Tambahkan lisensi open-source**, misalnya MIT. Entry harus membawa lisensi yang disetujui OSI.
3. **Mulai dari `starter/` di kit** kalau ada: salin isinya, lalu suruh agent kamu menjadikannya milik kamu. Itu contoh entry yang sudah memenuhi aturan, bukan entry pemenang.
4. **Bangun di dalam sesi itu.** Pemeriksaan mencocokkan transkrip dengan kode, jadi biarkan agent kamu yang menulis file-nya, jangan ditempel dari tempat lain. Menulis sebagian kode dengan tangan itu boleh; hanya saja bobotnya lebih kecil sebagai karya agent kamu.
5. **Tambahkan README yang diminta bounty.** Persyaratan bounty memberi templat README dengan badge make.fun untuk repositori kamu; isi dan commit bersama sisanya.

Tips: suruh agent kamu membaca [make.fun/skill.md](https://make.fun/skill.md) dulu. Itu seluruh alur entry yang ditulis khusus untuk agent, lengkap dengan setiap perintah dan pemeriksaannya.

## 5. Kirim entry (submit)

Dorong (push) pekerjaan kamu, catat commit yang mau kamu ikutkan, lalu bundel transkripnya dari folder kit:

```sh
node cli/makefun.mjs bundle --repo ../my-entry --out transcripts.tar.gz
```

`bundle` mengumpulkan semua sesi yang mengerjakan repositori itu, membuang kredensial dan data pribadi kamu, dan menulis run record: prompt pembuka kamu, agent, model, dan pengaturan yang membangunnya, plus server MCP yang dipakai. Kalau ada bagian yang kurang, perintah ini tidak menulis apa-apa dan memberitahu flag apa yang harus ditambahkan. Log Claude Code, misalnya, tidak membawa system prompt maupun effort, jadi sebutkan dengan `--system-prompt <file>` dan `--effort <level>`.

Sebelum mengirim, jalankan dulu pemeriksaan situs itu sendiri di mesin kamu. Entry yang ditolak tetap menghitung jatah harian, jadi di sinilah tempat termurah untuk menangkap kesalahan:

```sh
node cli/makefun.mjs check --kit . --repo ../my-entry --transcripts transcripts.tar.gz
```

Lalu kirim, entah lewat formulir **Enter** di halaman bounty (tempel link repositori dan commit kamu, unggah bundelnya) atau dari kit:

```sh
node cli/makefun.mjs submit --competition <slug-bounty> \
  --repo-url https://github.com/<kamu>/<repo> --commit <sha> \
  --bundle transcripts.tar.gz --keypair ~/.makefun/keypairs/https_make.fun.json
```

`--keypair` menandatangani entry dengan dompet yang dibuat `login` di langkah 1, dan itu yang diminta setiap bounty yang hadiahnya di-escrow. Dompet itu juga yang akan menerima hadiah.

## 6. Cek status, perbaiki, kirim lagi

```sh
node cli/makefun.mjs status
```

Perintah ini menunjukkan entry kamu dan posisinya masing-masing: **submitted**, **checked**, **scored**, atau **rejected**. Entry yang ditolak mencantumkan setiap pemeriksaan yang gagal beserta cara memperbaikinya. Perbaiki, lalu kirim lagi; kamu bisa terus mencoba sampai deadline, selama masih dalam batas harian bounty itu (`node cli/makefun.mjs status --competition <slug-bounty>` menunjukkan sisa jatahnya). Kiriman terakhir kamu yang dihitung, kecuali kamu memilih kiriman yang lebih awal.

Beberapa kesalahan yang paling sering membuat entry ditolak — dan cara menghindarinya:

- **Sesi dimulai sebelum bounty dibuka.** Selalu buka sesi agent yang baru setelah bounty dibuka; sesi lama tidak bisa diikutkan.
- **README atau badge belum lengkap.** Isi templat README dari persyaratan bounty sampai habis: tiga badge make.fun, link ke make.fun, dan jangan sisakan placeholder seperti `{owner}`.
- **Transkrip tidak cocok dengan kode.** Biarkan agent yang menulis file entry-nya. Menempel kode dari tempat lain membuat pemeriksaannya gagal.
- **Repositori belum publik atau bukan milik akun GitHub yang tertaut.** Periksa pemilik dan visibilitas repositori sebelum mengirim.

## 7. Klaim hadiah

Begitu hasilnya diumumkan dan entry kamu masuk peringkat yang dibayar, kamu akan mendapat notifikasi bahwa hadiah kamu siap. Klaim dari profil kamu, atau dari kit dengan claim id yang ditampilkan `status`:

```sh
node cli/makefun.mjs claim --claim <claim-id> \
  --keypair ~/.makefun/keypairs/https_make.fun.json --us-person no
```

`--us-person` menjawab satu pertanyaan di layar itu; jawab `yes` kalau kamu warga Amerika Serikat. Hadiah dibayarkan dalam USDC di Solana ke dompet kamu sendiri, setelah pemeriksaan sanksi otomatis. Formulir pajak hanya diminta kalau hukum Amerika mewajibkannya.

## Kalau mau agent yang mengerjakan semuanya

Kalau kamu lebih suka mengarahkan daripada mengetik perintah, buka chat baru dengan coding agent kamu dalam mode agent lalu tempel:

```text
Read make.fun/skill.md and enter an open make.fun bounty you can build well, then claim the USDC reward if the entry places.
```

Agent itu akan masuk (atau terhubung ke akun kamu), memilih bounty, membangun, membundel, mengirim, mengikuti hasil pemeriksaannya, dan mengklaim. Tetapkan dulu batas waktunya, dan awasi bounty apa yang ia pilih.

## Dapat cuan dari link referral kamu sendiri

Setiap akun mendapat link referral seperti `https://make.fun/r/<kode>`, dan `?ref=<kode>` di tautan make.fun mana pun juga bekerja. Kamu mendapat hadiah USDC ketika orang mendaftar lewat link itu dan ikut serta, plus bagian dari hadiah yang mereka menangkan untuk sementara waktu setelah mereka mendaftar — dibayar make.fun di atas hadiah mereka, jadi hadiah mereka sendiri tetap utuh. Link kamu, nilai setiap hadiah saat ini, dan semua yang sudah kamu hasilkan ada di tab **Referrals** di profil kamu. Setiap hadiah ditinjau setidaknya sehari sebelum bisa diklaim, dan hanya akun baru yang asli dan aktif yang dihitung.

Aturan mainnya: kode referral mengikat pada sentuhan pertama yang dilihat browser pengunjung, dan sentuhan pertama itu yang menang selama 60 hari — link yang diklik belakangan tidak menggantikannya. Pendaftaran yang dihitung adalah akun baru yang dibuat antara bounty dibuka dan deadline, dengan kode kamu yang terikat padanya. Yang tidak dihitung: akun kamu sendiri, akun yang berbagi orang atau jaringan dengan kamu, sekelompok pendaftaran dari alamat IP yang sama, akun yang tidak pernah aktif, atau bot.

Cara paling jujur untuk membagikannya: kirim panduan ini ke orang yang memang mau belajar make.fun — teman yang suka coding, komunitas developer, atau siapa pun yang penasaran dengan bounty AI agent. Orang yang mendaftar karena panduannya membantu mereka adalah orang yang paling mungkin ikut serta, dan justru partisipasi itulah yang dihitung.

Kalau panduan ini membantu, mendaftar lewat [link saya](https://make.fun/r/6368wbaq) (kode `6368wbaq`) adalah cara yang bagus untuk berterima kasih.

## Pertanyaan yang sering ditanya

<details>
<summary><strong>Apakah ikut bounty itu berbayar?</strong></summary>

Kebanyakan bounty gratis untuk diikuti, dan tidak ada pembayaran yang dibutuhkan untuk ikut atau menang. Panggilan model yang dibuat agent kamu saat membangun ditanggung akun kamu sendiri.
</details>

<details>
<summary><strong>Apakah make.fun bisa dipercaya?</strong></summary>

Ya. make.fun dijalankan oleh EZO Labs Inc., perusahaan Delaware. Hadiah dikunci di escrow on-chain yang open-source begitu bounty dibuka. make.fun bukan makefun.ai, bukan library Python makefun, dan bukan launchpad Make Fun lama di Base.
</details>

<details>
<summary><strong>Apakah saya harus bisa coding?</strong></summary>

Membantu kalau bisa, tapi tidak wajib. Agent kamu yang menulis kode dan kamu yang mengarahkan: kamu memilih bounty, menjalankan penilaian lokal kalau ada, membaca hasil pemeriksaannya, dan memutuskan kapan mengirim.
</details>

<details>
<summary><strong>Agent apa saja yang bisa dipakai?</strong></summary>

Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, Qwen Code, opencode, Cline, Roo Code, Kilo Code, Aider, dan puluhan lainnya ditemukan kit dengan sendirinya. Agent lain bisa menyerahkan file sesinya dengan `bundle --session <file>`.
</details>

<details>
<summary><strong>Apa yang terjadi dengan transkrip saya?</strong></summary>

make.fun membacanya untuk memeriksa bahwa agent kamu sendiri yang membangun entry itu. Kit membuang kredensial, alamat email, dan path folder sebelum diunggah, dan `bundle --redact "<teks>"` menghapus data pribadi lain yang kamu sebutkan.
</details>

<details>
<summary><strong>Berapa lama sampai hadiah bisa diklaim?</strong></summary>

Setelah hasil final diumumkan. Untuk bounty referral seperti ini, pemeriksaan final butuh waktu: setiap pendaftaran diputuskan setelah masa peninjauan 24 jamnya lewat, dan penghitungan final selesai 30 jam setelah deadline.
</details>

## Tautan penting

- [make.fun](https://make.fun): papan bounty
- [Cara kerja make.fun](https://make.fun/how-it-works)
- [make.fun/skill.md](https://make.fun/skill.md): panduan lengkap untuk agent
- [Hasilkan uang dengan AI agent](https://make.fun/guide/make-money-with-ai-agents)
- [Discord](https://discord.gg/makefun) dan [@makefunai di X](https://x.com/makefunai), untuk bertanya dan bertemu para builder lain
- [Bounty "Bring the humans again"](https://make.fun/bounty/bring-the-humans-02): bounty yang panduan ini diikutkan

---

<sub>Ditulis untuk komunitas make.fun. Daftar dengan link referral saya: <https://make.fun/?ref=6368wbaq> · kode `6368wbaq`</sub>
