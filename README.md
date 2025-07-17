````markdown
# 🤖 SLYDO: Smart Learning Document Chatbot

**SLYDO** adalah chatbot cerdas berbasis dokumen yang memungkinkan pengguna untuk mengunggah file `.pptx`, `.pdf`, atau `.docx`, lalu bertanya apa saja terkait konten dokumen tersebut. Chatbot ini dirancang untuk membantu proses belajar, memahami materi presentasi, atau menghasilkan soal latihan secara otomatis.

---

## ✨ Fitur Utama

- 📂 **Dukungan File**: Mendukung `.pptx`, `.pdf`, dan `.docx`
- 🧠 **Chat AI**: Bertanya langsung berdasarkan isi dokumen
- 🎤 **Input Suara**: Ajukan pertanyaan dengan suara
- 🔈 **TTS (Text-to-Speech)**: Balasan AI bisa dibacakan
- 🖼️ **Preview Slide/Halaman**: Tampilkan gambar dari dokumen
- 🧾 **Riwayat Chat & Prompt Cepat**: Navigasi percakapan dan gunakan template pertanyaan instan

---

## 🚀 Instalasi & Jalankan

### 1. Clone repo ini
```bash
git clone https://github.com/yourusername/slydo-chatbot.git
cd slydo-chatbot
````

### 2. Install dependencies

Pastikan Python 3.8+ sudah terpasang.

```bash
pip install -r requirements.txt
```

### 3. Siapkan Poppler & LibreOffice

* **Poppler** (untuk konversi PDF ke gambar):
  Download dan ekstrak dari: [https://github.com/oschwartz10612/poppler-windows/releases](https://github.com/oschwartz10612/poppler-windows/releases)
  Lalu update path di variabel `POPPLER_PATH` pada kode.

* **LibreOffice** (untuk konversi PPTX ke PDF):
  Download: [https://www.libreoffice.org/download](https://www.libreoffice.org/download)
  Lalu update path di variabel `LIBREOFFICE_PATH`.

### 4. Jalankan aplikasi

```bash
python chatbot.py
```

---

## 🛠️ Struktur Proyek

```
slydo-chatbot/
│
├── chatbot.py             # Script utama (berbasis Gradio)
├── requirements.txt       # Daftar dependensi Python
├── output/                # Folder output gambar & teks hasil ekstraksi
├── README.md              # Dokumentasi proyek
```

---

## 📦 Dependencies

* `gradio`
* `speechrecognition`
* `pyttsx3`
* `python-pptx`
* `python-docx`
* `pdf2image`
* `Pillow`
* `requests`

> ✅ Semua paket sudah didefinisikan dalam `requirements.txt`.

---

## 🔐 API Key

SLYDO menggunakan layanan dari **OpenRouter.ai** untuk koneksi ke LLM (Language Model). Anda dapat menggunakan model gratis `deepseek/deepseek-r1:free` atau mengganti model/API key sesuai kebutuhan.

Contoh bagian kode:

```python
"Authorization": "Bearer sk-or-...."
```

---

## 🧪 Contoh Prompt Cepat

* 📋 **Ringkasan** → `"Buat ringkasan singkat dari dokumen ini."`
* 🔍 **Penjelasan Slide** → `"Jelaskan isi dari slide 3."`
* ❓ **Pertanyaan Latihan** → `"Buat 3 soal latihan dari materi ini."`
* 🖼️ **Makna Gambar** → `"Jelaskan makna gambar pada slide atau halaman."`
* 📊 **Interpretasi Data** → `"Apa interpretasi dari grafik atau data yang ditampilkan?"`

---

## 🖼️ Tampilan Antarmuka

> (Tambahkan screenshot jika tersedia)

---

## 📜 Lisensi

Proyek ini dilisensikan di bawah **MIT License**.

---

## 🙌 Kontribusi

Pull request sangat disambut!
Untuk ide, perbaikan bug, atau usulan fitur baru, silakan buka **issue** terlebih dahulu.

---

## 📬 Kontak

* **Dibuat oleh**: Deven Utama
* **Email**: [utamadeven88@gmail.com](mailto:utamadeven88@gmail.com)
* **GitHub**: [@Dvnu8](https://github.com/Dvnu8)

---

Terima kasih telah menggunakan SLYDO! 🎓📚

```

---

### 📌 Tips

Simpan teks di atas sebagai file `README.md` di direktori proyek Anda. Markdown ini sudah kompatibel dengan GitHub dan akan tampil rapi secara otomatis.

Jika Anda butuh `requirements.txt`, tinggal beri tahu, saya bisa bantu buatkan berdasarkan dependensi yang dipakai.
```
