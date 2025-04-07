
# firmware-zte-670
Firmware GPON ZTE F670 V2.0, Masih default/bawaan ISP Indonesia.
 - Tambah/Hapus Wan: ✔
 - Edit Serial Number (SN): ❌

  ![image](https://github.com/user-attachments/assets/4cd307d8-0f30-4e67-b61a-6241ff8f972a)
  
 **Spesifikasi:**
 - Model:	F670
 - Hardware Version:	V2.0
 - Software Version:	V6.0.10P3N24
 - Boot Loader Version:	V6.0.10P10N1
 - SPI NAND FLASH MEMORY: FM25S01A 3.3V 1G-BIT


**Firmware info (F670.bin)**
| DECIMAL | HEXADECIMAL | DESCRIPTION                                                  |
|---------|-------------|--------------------------------------------------------------|
| 134928  | 0x20F10     | device tree image (dtb)                                      |
| 136192  | 0x21400     | device tree image (dtb)                                      |
| 203632  | 0x31B70     | CRC32 polynomial table - little endian                       |
| 229101  | 0x37EED     | Sega MegaDrive/Genesis raw ROM dump Name: "1CWSIGA 128MiB 3" |
| 9043968 | 0x8A0000    | JFFS2 filesystem - little endian                             |

**F670-JFFS2.zip**

Adalah file JFFS2 yang sudah di extract, untuk UI ada di folder `flag_type/httpd` dan fungsi yang berhubungan dengan konfigurasi hardware atau dekripsi config.bin mungkin ada di file `*.ko` seperti `kmodule/zte_gpon.ko`

![image](https://github.com/user-attachments/assets/1990522f-6ccf-4cac-b421-cbbe829eb699)

## Cara Dump dan Flash Firmware

Bahan:
- Modul CH341A Programmer
- Kawat email 0,3 mm
- Software Ch341a Programmer (NeoProgrammer) V2.2.0.10

![image](https://github.com/user-attachments/assets/793d50b1-77bf-48db-a3ff-32c40bbad728)

**Cara Dump:**
- Hubungkan IC FM25S01A di F670 ke modul CH341A dengan kawat email
- Buka NeoProgrammer lalu klik `detect`
- di jendela Popup cari atau masukan `FM25S01A` dan `Read IC`
- Setelah selesai di Read, file nya bisa di `Save` dengan format `.bin` dan dapat extract dengan `binwalk`

**Cara Flash:**
- Buka file `.bin`
- Klik `Write IC`
- 
## TO-DO (dibutuhkan bantuan):
- Ubah SN ❌
- Ubah GPON ke EPON ❌
