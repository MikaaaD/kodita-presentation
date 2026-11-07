# KODITA OS

Materi belajar koding KODITA dalam bentuk desktop komputer. Setiap folder dan file membuka materi baru.

- `index.html`: KODITA OS (presentasi utama)
- `slides/index.html`: versi slide biasa Module 01 Web Dev

## Cara pakai
- Double-click folder untuk membuka isinya (di HP cukup tap sekali)
- Double-click file `.slide` untuk membuka materi
- Pindah slide pakai tombol panah atau keyboard ← →
- Tombol **▶ demo** di taskbar menjalankan kursor otomatis

## Cara menambah materi
Buka `index.html`, cari bagian `const FS = [` di awal `<script>`.

1. Cari file modul yang mau diisi, misalnya `{id:'web3',name:'03_layout.slide',type:'slide',lock:true}`
2. Hapus `lock:true`, lalu tambahkan `slides:[ ... ]`
3. Jenis slide yang bisa dipakai:

| Jenis | Isi |
|---|---|
| `cover` | `tag`, `title`, `hl` (judul ungu), `lead` |
| `list` | `tag`, `title`, `items` (daftar poin) |
| `code` | `tag`, `title`, `lang` (`html`/`lua`), `code`, lalu `preview` (HTML) atau `output` (teks terminal) |
| `live` | `tag`, `title`, `starter` (kode awal yang bisa diedit peserta) |
| `quiz` | `tag`, `title`, `opts` (pilihan), `ok` (nomor jawaban benar, mulai dari 0), `msg` |
| `done` | `title`, `progress`, `total`, `next` |

Contoh:
```js
{t:'list',tag:'MISSION BRIEFING',title:'Target misi hari ini',items:['Poin 1','Poin 2']}
```

Dibuat oleh tim KODITA.
