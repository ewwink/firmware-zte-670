
# firmware-zte-670
Firmware GPON ZTE F670 V2.0, Masih default/bawaan ISP Indonesia.
 - Tambah/Hapus Wan: ✔
 - Edit Serial Number (SN): ❌
  
 **Spesifikasi:**
 - Model:	F670
 - Hardware Version:	V2.0
 - Software Version:	V6.0.10P3N24
 - Boot Loader Version:	V6.0.10P10N1

**Firmware info (F670.bin)**
| DECIMAL | HEXADECIMAL | DESCRIPTION                                                  |
|---------|-------------|--------------------------------------------------------------|
| 134928  | 0x20F10     | device tree image (dtb)                                      |
| 136192  | 0x21400     | device tree image (dtb)                                      |
| 203632  | 0x31B70     | CRC32 polynomial table - little endian                       |
| 229101  | 0x37EED     | Sega MegaDrive/Genesis raw ROM dump Name: "1CWSIGA 128MiB 3" |
| 9043968 | 0x8A0000    | JFFS2 filesystem - little endian                             |

**F670-JFFS2.zip**

Adalah file JFFS2 yang sudah di extract, untuk UI ada di folder `flag_type/httpd` dan fungsi yang berhubungan dengan konfigurasi dengan hardware kemungkinan ada di file `kmodule/zte_gpon.ko`

![image](https://github.com/user-attachments/assets/1990522f-6ccf-4cac-b421-cbbe829eb699)

**TO-DO (dibutuhkan bantuan):**
- Ubah SN ❌
- Ubah GPON ke EPON ❌
