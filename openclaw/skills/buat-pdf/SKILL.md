---
name: buat-pdf
description: Membuat file PDF dari konten apa pun dan mengirimkannya ke chat. Pakai setiap kali diminta membuat PDF.
---

Ikuti langkah ini persis. Jangan pakai cara lain (bukan Python, bukan weasyprint, bukan screenshot).

1. Tulis kontennya sebagai file HTML di folder /home/budi/.openclaw/workspace dengan alat write.
2. Jalankan perintah shell ini lewat alat untuk menjalankan perintah (di Code Mode cari dengan catalog.search("shell command"); jangan pakai require):
   google-chrome --headless --disable-gpu --print-to-pdf="/home/budi/.openclaw/workspace/NAMA.pdf" "/home/budi/.openclaw/workspace/NAMA.html"
3. Periksa bahwa file PDF itu benar-benar ada. Kalau tidak ada, laporkan error aslinya dan berhenti. Jangan bilang berhasil.
4. Kirim file PDF (bukan HTML) ke chat asal permintaan dengan alat message, action send, media berisi path PDF.
