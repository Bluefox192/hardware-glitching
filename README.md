# 🔧 Hardware Glitching – by Bluefox192

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Open Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen)](https://github.com/Bluefox192/hardware-glitching/issues)
[![Project Status](https://img.shields.io/badge/status-active-blue)](#-status-proyek)
[![Made with Arduino](https://img.shields.io/badge/made%20with-arduino-blue?logo=arduino)](https://www.arduino.cc)
[![Tool: CH341A](https://img.shields.io/badge/tool-CH341A-yellow)](https://github.com/Bluefox192/hardware-glitching)
![Open Issues](https://img.shields.io/github/issues/Bluefox192/hardware-glitching.svg)
![Last Commit](https://img.shields.io/github/last-commit/Bluefox192/hardware-glitching)
![PR Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

> ⚡ Eksplorasi open-hardware untuk *fault injection* terhadap mikrokontroler.  
> Fokus pada **voltage glitching** menggunakan Arduino Nano sebagai glitch generator,  
> serta eksperimen awal dengan **CH341A** untuk dumping firmware via SPI.  
> Ditujukan untuk edukasi, riset keamanan embedded system, dan eksplorasi teknik serangan perangkat keras.

---

## 🧠 Tentang Proyek

**Hardware Glitching** (a.k.a. Fault Injection) adalah teknik ampuh yang digunakan untuk menerobos mekanisme keamanan dengan menginduksi kesalahan pada eksekusi mikrokontroler.  
Proyek ini mengeksplorasi teknik **gangguan tegangan** menggunakan perangkat berbiaya rendah seperti **Arduino Nano**, dan kini berkembang ke eksperimen dumping menggunakan **CH341A SPI programmer**.

---

## 🛠️ Progress Saat Ini

| Tanggal | Update |
|--------|--------|
| ✅ Juli 2025 | Rangkaian glitch generator Arduino berfungsi |
| ✅ Juli 2025 | Uji coba dasar voltage glitch terhadap ATmega328 |
| 🔜 Agustus 2025 | **Pembelian dan pengujian CH341A programmer** |
| ⏳ Agustus–September | Dump firmware dari chip SPI eksternal (W25Q, 24C) |
| 📌 Planned | Reverse firmware hasil dump dan injeksi kembali |

---

## 📁 Struktur Direktori

```

/docs/       → Penjelasan eksperimen & teori
/firmware/   → Firmware Arduino Nano untuk glitch trigger
/hardware/   → Rangkaian, skematik, dan layout PCB
/logs/       → Catatan eksperimen harian (dipisahkan)
/tools/      → Gambar alat bantu dan dokumentasi visual

```

📖 **Log eksperimen lengkap tersedia di folder [`/logs/`](logs/)**

---

## 🎯 Fokus Eksperimen

- ⚡ Voltage glitching terhadap ATmega328 dan mikrokontroler lain
- ⏱ Timing injection & kontrol delay presisi
- 💾 Dumping firmware dari SPI flash via CH341A
- 🧬 Pengaruh terhadap instruksi `jmp`, `ldi`, dsb.
- 🔍 Analisis hasil dump menggunakan `binwalk`, `Ghidra`, dan `xxd`

---

## 🔭 Rencana Kedepan

- [ ] Menyusun toolchain lengkap CH341A di Linux
- [ ] Katalog chip SPI umum (datasheet, pinout)
- [ ] Dump firmware dari perangkat nyata (router, keyboard, gadget)
- [ ] Analisis firmware & patch (reversing dasar)
- [ ] Simulasi serangan pada bootloader dan proteksi memori
- [ ] Penggabungan dengan logic analyzer dan oscilloscope sederhana

---

## 💡 Use Cases

- Evaluasi keamanan mikrokontroler terhadap fault injection
- Edukasi teknik hardware reverse engineering
- Eksplorasi teknik glitch untuk bypass proteksi bootloader atau fuses
- Dump firmware perangkat embedded / consumer electronics

---

## 🚀 Status Proyek

- 🔧 **Aktif dikembangkan** sejak Juli 2025
- 🧪 Eksperimen dasar glitching telah dimulai
- 🛍️ **CH341A segera dibeli untuk dumping firmware SPI**
- 📚 Dokumentasi dan tooling sedang disusun bertahap
- 📌 Roadmap publik akan diperbarui rutin

---

## 🤝 Kontribusi

Proyek ini terbuka untuk siapa saja yang tertarik di bidang:

- 🔐 Embedded Security
- 🔍 Reverse Engineering
- 💻 Hardware Hacking
- 📢 Open Research & Edukasi

Ingin berdiskusi atau berkolaborasi?
- 🧵 Buka [Issue](https://github.com/Bluefox192/hardware-glitching/issues)
- 🔀 Lakukan fork & ajukan Pull Request seperti biasa

---

## ⚠️ Etika & Legal

> Proyek ini **hanya untuk riset dan edukasi**.  
> Segala aktivitas harus dilakukan pada perangkat yang kamu miliki dan kontrol secara legal.  
> Penulis tidak bertanggung jawab atas penyalahgunaan terhadap sistem nyata atau produksi.

---

## 📬 Contact

Made with ❤️ by [Bluefox192](https://github.com/bluefox192)  
For questions or collaborations: [Bluefox192](https://github.com/bluefox192)

---

## 📄 Lisensi

Lisensi: [MIT License](LICENSE)  
© 2025 [Bluefox192](https://github.com/Bluefox192)

---

> “If you can glitch it, you can understand it.”  
> — Fault injection isn’t just hacking — it’s learning how things fail, and why.

---
