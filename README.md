🤖 SLYDO: Smart Learning Document Chatbot
SLYDO adalah chatbot cerdas berbasis dokumen yang memungkinkan pengguna untuk mengunggah file .pptx, .pdf, atau .docx, lalu bertanya apa saja terkait konten dokumen tersebut. Chatbot ini dirancang untuk membantu proses belajar, memahami materi presentasi, atau menghasilkan soal latihan secara otomatis.

✨ Fitur Utama
📂 Dukungan File: Mendukung .pptx, .pdf, dan .docx

🧠 Chat AI: Bertanya langsung berdasarkan isi dokumen

🎤 Input Suara: Ajukan pertanyaan dengan suara

🔈 TTS (Text-to-Speech): Balasan AI bisa dibacakan

🖼️ Preview Slide/Halaman: Tampilkan gambar dari dokumen

🧾 Riwayat Chat & Prompt Cepat: Navigasi percakapan dan gunakan template pertanyaan instan

🚀 Instalasi & Jalankan
1. Clone repo ini
bash
Copy
Edit
git clone https://github.com/yourusername/slydo-chatbot.git
cd slydo-chatbot
2. Install dependencies
Pastikan Python 3.8+ sudah terpasang.

bash
Copy
Edit
pip install -r requirements.txt
3. Siapkan Poppler & LibreOffice
Poppler (untuk konversi PDF ke gambar):
Download dan ekstrak dari: https://github.com/oschwartz10612/poppler-windows/releases
Update path di variabel POPPLER_PATH.

LibreOffice (untuk konversi PPTX ke PDF):
Download: https://www.libreoffice.org/download
Update path di variabel LIBREOFFICE_PATH.

4. Jalankan aplikasi
bash
Copy
Edit
python chatbot.py
🛠️ Struktur Proyek
bash
Copy
Edit
slydo-chatbot/
│
├── chatbot.py             # Script utama (berbasis Gradio)
├── requirements.txt       # Daftar dependensi Python
├── output/                # Folder output gambar & teks hasil ekstraksi
├── README.md              # Dokumentasi proyek
📦 Dependencies
gradio

speechrecognition

pyttsx3

python-pptx

python-docx

pdf2image

Pillow

requests

✅ Semua paket didefinisikan dalam requirements.txt

🔐 API Key
SLYDO menggunakan OpenRouter.ai untuk koneksi ke LLM. Anda bisa menggunakan model gratis (deepseek/deepseek-r1:free) atau mengganti model/API key Anda sendiri.

Ganti Authorization di bagian:

python
Copy
Edit
"Authorization": "Bearer sk-or-...."
🧪 Contoh Prompt Cepat
📋 Ringkasan → "Buat ringkasan singkat dari dokumen ini."

🔍 Penjelasan Slide → "Jelaskan isi dari slide 3."

❓ Pertanyaan Latihan → "Buat 3 soal latihan dari materi ini."

🖼️ Makna Gambar → "Jelaskan makna gambar pada slide atau halaman."

📊 Interpretasi Data → "Apa interpretasi dari grafik atau data yang ditampilkan?"

🖼️ Tampilan Antarmuka

📜 Lisensi
Proyek ini dilisensikan di bawah MIT License.

🙌 Kontribusi
Pull request sangat disambut!
Untuk ide, bug, atau fitur baru, silakan buat issue terlebih dahulu.

📬 Kontak
Dibuat oleh Deven Utama
Email: utamadeven88@gmail.com
GitHub: @Dvnu8