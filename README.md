# 🏎️ Engine Telemetry & Thermal Monitoring Simulation

> **Language / Bahasa:** [English](#english) | [Bahasa Indonesia](#bahasa-indonesia)

---

## English

### 📌 Overview
An embedded sensor data acquisition (DAQ) and telemetry prototype node modeled for Formula Student internal combustion engine (ICE) race cars. 

This project simulates real-time driver throttle inputs and calculates dynamic engine coolant thermal fluctuations, complete with an automated overheat protection logic and serial telemetry data broadcasting for pit-stop monitoring.

### 🚀 Live Interactive Simulation
You can test and interact with the live hardware circuit directly in your browser:  
👉 **[Click Here to Run Wokwi Simulation](https://wokwi.com/projects/479754977530363905)**

### ✨ Key Features
- **Throttle Position Sensor (TPS) Acquisition:** Reads analog inputs (0–100%) simulating dynamic accelerator pedal travel.
- **Engine Coolant Temperature (ECT) Dynamic Modeling:** Simulates real-time engine thermal rise correlated with throttle load.
- **Fail-Safe Alert Logic:** Automatically triggers an alert indicator (LED pin 13) and flags critical warning packets when coolant temperature breaches safety thresholds (>95°C).
- **Serial Telemetry Stream:** Formats and broadcasts structured data packets via Serial at a 2Hz refresh rate for crew diagnostics.

### 🛠️ Hardware Pinout & Tech Stack
- **Platform:** Arduino Uno / ATmega328P (Wokwi Simulation)
- **Language:** C/C++
- **Wiring Configuration:**
  - `A0` : Potentiometer (Simulated Throttle Position Sensor)
  - `Pin 13` : Digital Output (Overheat Dashboard Warning LED)

---

## Bahasa Indonesia

### 📌 Ringkasan Proyek
Prototipe akuisisi data sensor (*Data Acquisition / DAQ*) dan node telemetri *embedded* yang dimodelkan untuk mobil balap Formula Student berbasis mesin bensin (*Internal Combustion Engine / ICE*).

Proyek ini mensimulasikan pembacaan injakan pedal gas pengemudi (*throttle*) dan memodelkan dinamika fluktuasi suhu air radiator mesin (*Engine Coolant Temperature*), lengkap dengan logika pengaman otomatis saat terjadi *overheat* serta pengiriman data telemetri serial untuk pemantauan kru di *pit stop*.

### 🚀 Simulasi Interaktif Langsung
Kamu bisa menguji dan berinteraksi langsung dengan rangkaian elektronika ini di browser:  
👉 **[Klik di Sini untuk Menjalankan Simulasi Wokwi](https://wokwi.com/projects/479754977530363905)**

### ✨ Fitur Utama
- **Pembacaan Sensor Bukaan Gas (TPS):** Membaca input analog (0–100%) yang merepresentasikan pergerakan pedal gas secara dinamis.
- **Pemodelan Termal Mesin (ECT):** Memodelkan respons kenaikan temperatur pendingin mesin secara dinamis berdasarkan beban injakan gas.
- **Logika Pengaman Otomatis (*Fail-Safe*):** Mengaktifkan lampu peringatan bahaya di dashboard (LED Pin 13) dan memicu status kritis ketika temperatur pendingin melebihi batas aman (>95°C).
- **Transmisi Telemetri Serial:** Mengirimkan paket data terstruktur secara *real-time* dengan frekuensi 2Hz (dua kali per detik) ke monitor *pit stop*.

### 🛠️ Konfigurasi Pin & Teknologi
- **Platform:** Arduino Uno / ATmega328P (Simulasi Wokwi)
- **Bahasa:** C/C++
- **Konfigurasi Rangkaian:**
  - `A0` : Potensiometer (Simulasi *Throttle Position Sensor / TPS*)
  - `Pin 13` : Output Digital (Lampu Indikator Peringatan *Overheat*)

---
*Developed by NaufalAurelioE.*
