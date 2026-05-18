# Praktikum Sistem Digital - Pertemuan 8
## Modul: Gerbang Logika Tinkercad

Tinkercad merupakan platform berbasis *web app* untuk simulasi rangkaian digital maupun analog. Pada praktikum sebelumnya kita sudah mempelajari gerbang logika sebagai dasar rangkaian elekronika, maka untuk pertemuan kali ini kita akan menyimulasikan rangkaian LED sederhana menggunakan Tinkercad. Total ada 7 gerbang logika yang diujikan menggunakan seri IC 74HC:
- AND (IC 74HC08)
- OR (IC 74HC32)
- NOT (IC 74HC04)
- NAND (IC 74HC00)
- NOR (IC 74HC02)
- XOR (IC 74HC86)
- XNOR (IC 74HC86 [XOR] + IC 74HC04 [NOT])

Semua rangkaian dipasangkan dengan Power supply DC, LED berwarna merah, resistor 220ohm, dan DIP switch. 

<br>

### A. AND

<img width="313,5" height="265,5" alt="Screenshot 2026-05-17 130013" src="https://github.com/user-attachments/assets/579299f7-d73f-4be8-9fea-54fbec247f0c" />

Logika gerbang AND adalah semua input harus HIGH agar output-nya HIGH. Pada rangkaian, terlihat bahwa input berasal dari DIP switch 1 dan 2 atau anggap saja A dan B. Jika tegangan di-set 5V, lalu A dan B dinyalakan, maka LED akan menyala.

Berikut tabel kebenarannya:
| A (1) | B (2) | OUTPUT LED |
|-------|-------|------------|
|   0   |   0   |  LOW (OFF) |
|   0   |   1   |  LOW (OFF) |
|   1   |   0   |  LOW (OFF) |
|   1   |   1   |  HIGH (ON) |

<br>

### B. OR

<img width="321" height="265,5" alt="Screenshot 2026-05-17 130018" src="https://github.com/user-attachments/assets/a794002c-33bf-4548-a1cb-865a4c3627d5" />

Logika gerbang OR adalah salah satu input harus HIGH agar output-nya HIGH. Jika tegangan di-set 5V, lalu salah satu atau kedua A dan B dinyalakan, maka LED akan menyala.

Berikut tabel kebenarannya:
| A (1) | B (2) | OUTPUT LED |
|-------|-------|------------|
|   0   |   0   |  LOW (OFF) |
|   0   |   1   |  HIGH (ON) |
|   1   |   0   |  HIGH (ON) |
|   1   |   1   |  HIGH (ON) |

<br>

### C. NOT

<img width="309" height="247,5" alt="Screenshot 2026-05-17 130024" src="https://github.com/user-attachments/assets/323b43f9-8ae3-4421-b51e-d8404e980983" />

Logika gerbang OR adalah *inventer* atau pembalik. Terlihat bahwa hanya terdapat satu jalur input dari DIP switch. Jika tegangan di-set 5V, lalu switch dimatikan, maka LED akan menyala.

Berikut tabel kebenarannya:
| SWITCH | OUTPUT LED |
|--------|------------|
| 0      |  HIGH (ON) |
| 1      |  LOW (OFF) |

<br>

### D. NAND (NOT-AND)

<img width="300" height="258" alt="Screenshot 2026-05-17 130030" src="https://github.com/user-attachments/assets/7ebe69d1-be64-4ba3-a80d-abdce859cdcd" />

Logika gerbang NAND adalah output-nya kebalikan dari NAND. Jika tegangan di-set 5V, lalu salah satu atau kedua A dan B dimatikan, maka LED akan menyala.

Berikut tabel kebenarannya:
| A (1) | B (2) | OUTPUT LED |
|-------|-------|------------|
|   0   |   0   |  HIGH (ON) |
|   0   |   1   |  HIGH (ON) |
|   1   |   0   |  HIGH (ON) |
|   1   |   1   |  LOW (OFF) |

<br>

### E. NOR (NOT-OR)

<img width="312" height="265,5" alt="Screenshot 2026-05-17 130035" src="https://github.com/user-attachments/assets/0a06410a-a243-46c8-b3e9-f711f144d247" />

Logika gerbang NOR adalah output-nya kebalikan dari OR. Jika tegangan di-set 5V, lalu A dan B dimatikan, maka LED akan menyala.

Berikut tabel kebenarannya:
| A (1) | B (2) | OUTPUT LED |
|-------|-------|------------|
|   0   |   0   |  HIGH (ON) |
|   0   |   1   |  LOW (OFF) |
|   1   |   0   |  LOW (OFF) |
|   1   |   1   |  LOW (OFF) |

<br>

### F. XOR (EXCLUSIVE-OR)

<img width="312" height="265,5" alt="Screenshot 2026-05-17 130041" src="https://github.com/user-attachments/assets/42c2413d-f29f-45ae-9117-bced82305740" />

Logika gerbang XOR adalah semua input harus dalam kondisi berbeda agar output-nya HIGH. Jika tegangan di-set 5V, lalu salah satu A atau B dinyalakan, maka LED akan menyala.

Berikut tabel kebenarannya:
| A (1) | B (2) | OUTPUT LED |
|-------|-------|------------|
|   0   |   0   |  LOW (OFF) |
|   0   |   1   |  HIGH (ON) |
|   1   |   0   |  HIGH (ON) |
|   1   |   1   |  LOW (OFF) |

<br>

### G. XNOR (EXCLUSIVE-NOT-OR)

<img width="357" height="255" alt="Screenshot 2026-05-17 130047" src="https://github.com/user-attachments/assets/cf78f282-1674-4066-8ed8-5cf49f04a098" />

Logika gerbang XNOR adalah semua input harus dalam kondisi sama agar output-nya HIGH. Jika tegangan di-set 5V, lalu A dan B sama-sama dinyalakan atau dimatikan, maka LED akan menyala.

Berikut tabel kebenarannya:
| A (1) | B (2) | OUTPUT LED |
|-------|-------|------------|
|   0   |   0   |  HIGH (ON) |
|   0   |   1   |  LOW (OFF) |
|   1   |   0   |  LOW (OFF) |
|   1   |   1   |  HIGH (ON) |

<br>

### Referensi

#### Anggota Kelompok= Nama (NIM):
- Maeda Kamila Fatrah (H1H025013)
- Irsyad Amar Ramadhan (H1H025016)

[Link Tinkercad](https://www.tinkercad.com/things/b4zTZpq5OK3-pert8-praksisdig?sharecode=J_NMEL4Qnbh_BZo_YMhxg6CQbPzr_iyVJqiaEJcwUz8)
