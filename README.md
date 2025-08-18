# Welcome to Linux Directory Structure

![Linux-Directory-Structure](/img/lds.png)

## `/ - Root`

`en`
- Every single file and directory starts from the root directory.
- Only root user has write privilege under this directory.
- Please note that /root is root user's home directory, which is not same as /.

`ind`
- Setiap file dan direktori dimulai dari direktori root.
- Hanya pengguna root yang memiliki hak tulis di direktori ini.
- Perlu dicatat bahwa /root adalah direktori home untuk pengguna root, yang berbeda dengan /.   

## `/bin - User Binaries`

`en`
- Contains binary executables.
- Common linux commands you need to use in single-user modes are located under this directory.
- Commands used by all the users of the system are located here.
- For example: ps, ls, ping, grep, cp.

`ind`
- Berisi file biner yang dapat dieksekusi.
- Perintah Linux umum yang perlu digunakan dalam mode single-user berada di direktori ini.
- Perintah yang digunakan oleh semua pengguna sistem juga ada di sini.
- Contohnya: ps, ls, ping, grep, cp.

## `/sbin - System Binaries`

`en`
- Just like /bin, `/sbin` also contains binary executables.
- But, the linux commands located under this directory are used typically by system administrastor, for system maintenance purpose.
- For example: iptables, reboot, fdisk, ifconfig, swapon

`ind`
- Sama seperti /bin, `/sbin` juga berisi file biner yang dapat dieksekusi.
- Namun, perintah Linux yang ada di direktori ini biasanya digunakan oleh administrator sistem untuk keperluan pemeliharaan sistem.
- Contohnya: iptables, reboot, fdisk, ifconfig, swapon

## `/etc - Configuration Files`

`en`
- Contains configuration files required by all programs.
- This also startup and shutdown shell scripts used to start/stop individual programs.
- For example: /etc/resolv.conf, /etc/logrotate.conf

`ind`
- Berisi file konfigurasi yang dibutuhkan oleh semua program.
- Juga terdapat skrip shell untuk proses startup dan shutdown yang digunakan untuk memulai/menghentikan program tertentu.
- Contohnya: /etc/resolv.conf, /etc/logrotate.conf

## `/dev - Device Files`

`en`
- Contains device files.
- These include terminal devices, usb, or any attached to the system.
- For example: /dev/tty1, dev/usbmon0

`ind`
- Berisi file perangkat.
- Termasuk perangkat terminal, usb, atau perangkat lain yang terhubung ke sistem.
- Contohnya: /dev/tty1, dev/usbmon0

## `/proc - Process Information`

`en`
- Contains information about system process.
- This is a pseudo file system contain information about running process. For example: /prod/{pid} directory contains information about the process with that particular pid.
- For example: /proc/uptime

`ind`
- Berisi informasi tentang proses sistem.
- Ini adalah sistem file semu yang berisi informasi tentang proses yang sedang berjalan. Misalnya: direktori /proc/{pid} berisi informasi tentang proses dengan pid tertentu.
- Contohnya: /proc/uptime

## `/var - Variable Files`

`en`
- Var stands for variable files.
- Content of the files that are expected to grow can be found under this directory.
- This include --- System log files (/var/log); Packages and databases files (/var/lib); Emails(/var/mail); Print queues (/var/spool); Lock files(/var/lock); Temp files needed accros reboots (/var/tmp);

`ind`
- Var adalah singkatan dari variable files (file variabel).
- Isi file yang diperkirakan akan bertambah dapat ditemukan di direktori ini.
- Ini termasuk --- File log sistem (/var/log); File paket dan database (/var/lib); Email (/var/mail); Antrian cetak (/var/spool); File kunci (/var/lock); File sementara yang dibutuhkan saat reboot (/var/tmp);

## `/tmp - Temporary Files`

`en`
- Directory that contains temporary files created by system and users.
- Files under this directory are deleted when system is rebooted.

`ind`
- Direktori yang berisi file sementara yang dibuat oleh sistem dan pengguna.
- File di dalam direktori ini akan dihapus saat sistem di-reboot.

## `/usr - User Programs`

`en`
- Contains binaries, libraries, documentation, and source-code for second level programs.
- /usr/bin contains binary files for user program. If you can't find a user binary under /bin, look under /usr/bin. For example: at, awk, cc, less, scp.
- /usr/sbin contains binary files for system administrator. If you can't find a system binary under /sbin, look under /usr/sbin. For example: atd, cron, sshd, useradd, userdel
- /usr/lib contains libraries for /usr/bin and /usr/sbin.
- /usr/local contains users programs that you install from source. For example, when you install apache from source, it goes under /usr/local/apache2.

`ind`
- Berisi file biner, pustaka, dokumentasi, dan source code untuk program tingkat kedua.
- /usr/bin berisi file biner untuk program pengguna. Jika Anda tidak menemukan biner pengguna di /bin, carilah di /usr/bin. Contohnya: at, awk, cc, less, scp.
- /usr/sbin berisi file biner untuk administrator sistem. Jika Anda tidak menemukan biner sistem di /sbin, carilah di /usr/sbin. Contohnya: atd, cron, sshd, useradd, userdel.
- /usr/lib berisi pustaka untuk /usr/bin dan /usr/sbin.
- /usr/local berisi program pengguna yang Anda instal dari source. Misalnya, ketika Anda menginstal apache dari source, maka akan berada di /usr/local/apache2.

## `/home - Home Directories`
 
`en`
- Home directories for all users to store their personal files.
- For example: /home/john, /home/codemax.

`ind`
- Direktori home untuk semua pengguna untuk menyimpan file pribadi mereka.
- Contohnya: /home/john, /home/codemax.

## `/boot - Boot Loader Files`

`en`
- Contains boot loader related files.
- Kernel initrd, vmlinux, grub files are located under /boot.
- For example: initrd.img-2.6.32-34-generic

`ind`
- Berisi file-file yang berhubungan dengan boot loader.
- File kernel initrd, vmlinux, grub berada di dalam /boot.
- Contohnya: initrd.img-2.6.32-34-generic

## `/lib - System Libraries`   

`en`
- Contains library files that supports the binaries located under /bin and /sbin
- Libary filenames are either ld* or lib*.so.*
- For example: ld-2.11.1.so

`ind`
- Berisi file pustaka yang mendukung file biner yang ada di /bin dan /sbin.
- Nama file pustaka biasanya diawali dengan ld* atau lib*.so.*
- Contohnya: ld-2.11.1.so

## `/opt - Optional add-on Applications`

`en`
- Opt stands for optional.
- Contains add-on application from individual vendors.
- Add-on application should be installed under either /opt or /opt/sub-directory.

`ind`
- Opt adalah singkatan dari optional (opsional).
- Berisi aplikasi tambahan dari vendor tertentu.
- Aplikasi tambahan sebaiknya diinstal di /opt atau di sub-direktori /opt.

## `/mnt - Mount Directory`

`en`
- Temporary mount directory where sysadmins can mount filesystems.

`ind`
- Direktori mount sementara tempat sysadmin dapat me-mount filesystem.

## `/media - Removable Media Device`

`en`
- Temporary mount directory for removable files.
- For example: /media/cdrom for CD-ROM; /media/floppy for floppy drives

`ind`
- Direktori mount sementara untuk file yang dapat dilepas.
- Contohnya: /media/cdrom untuk CD-ROM; /media/floppy untuk floppy drive

## `srv - Service Data`

`en`
- Srv stands for service.
- Contains server spesific services related data.
- For example: /srv/cvs contains CVS related data.

`ind`
- Srv adalah singkatan dari service (layanan).
- Berisi data yang berkaitan dengan layanan server tertentu.
- Contohnya: /srv/cvs berisi data terkait CVS.

## Summary

`en`
### **`/ (Root)`**

* All files & folders start from here.
* Only the **root user** can write directly here.
* Don't get confused: `/` ≠ `/root` (the latter is the home directory for the root user).

---

### **`/bin` (User Binaries)**

* Contains **common commands** usable by all users.
* Example: `ls` (list directory), `cp` (copy file), `ping`.

---

### **`/sbin` (System Binaries)**

* Similar to `/bin`, but specifically for **system admin commands**.
* Example: `reboot`, `fdisk`, `ifconfig`.

---

### **`/etc` (Configuration Files)**

* Place for **system & program configuration files**.
* Example: `resolv.conf` (DNS), `logrotate.conf` (log settings).

---

### **`/dev` (Device Files)**

* Folder containing **hardware device files**.
* Example: `/dev/tty1` (terminal), `/dev/usbmon0` (USB).

---

### **`/proc` (Process Info)**

* Pseudo folder to view **currently running processes**.
* Example: `/proc/uptime` (system uptime), `/proc/1234` (info for process PID 1234).

---

### **`/var` (Variable Files)**

* Files that **always change/grow**.
* Example: `/var/log` (system logs), `/var/mail` (emails), `/var/spool` (print queue).

---

### **`/tmp` (Temporary Files)**

* Place for temporary files (automatically deleted on reboot).
* Example: unfinished download files.

---

### **`/usr` (User Programs)**

* Place for additional programs & libraries.
* `/usr/bin` → regular programs (e.g. `awk`, `scp`).
* `/usr/sbin` → admin programs (`sshd`, `cron`).
* `/usr/local` → programs **manually installed from source** (e.g. Apache from source).

---

### **`/home` (Home Directories)**

* Personal folders for each user.
* Example: `/home/arya`, `/home/john`.

---

### **`/boot` (Boot Files)**

* Important files for **system booting**.
* Example: kernel (`vmlinuz`), `grub`.

---

### **`/lib` (System Libraries)**

* Contains libraries used by `/bin` & `/sbin`.
* Example: `ld-2.11.1.so`.

---

### **`/opt` (Optional Apps)**

* Place for additional applications from third-party vendors.
* Example: `/opt/google/chrome`.

---

### **`/mnt` (Temporary Mount Point)**

* Temporary place to **mount filesystems**.
* Example: mount an external hard drive here.

---

### **`/media` (Removable Media)**

* Place for **automatically mounted** external media.
* Example: `/media/cdrom`, `/media/usb`.

---

### **`/srv` (Service Data)**

* Special data for **server services**.
* Example: `/srv/cvs` for CVS server data.

---

In summary:

* `/bin`, `/sbin` → commands
* `/etc` → configuration
* `/home` → user files
* `/var` → frequently changing data
* `/boot` → boot files
* `/dev` & `/proc` → hardware & process info
* `/mnt` & `/media` → storage mounts

`ind`
### **`/ (Root)`**

* Semua file & folder dimulai dari sini.
* Hanya **root user** yang bisa nulis langsung di sini.
* Jangan bingung: `/` ≠ `/root` (yang terakhir itu home khusus untuk user root).

---

### **`/bin` (User Binaries)**

* Berisi **perintah umum** yang bisa dipakai semua user.
* Contoh: `ls` (lihat isi folder), `cp` (copy file), `ping`.

---

### **`/sbin` (System Binaries)**

* Sama kayak `/bin`, tapi khusus **perintah admin sistem**.
* Contoh: `reboot`, `fdisk`, `ifconfig`.

---

### **`/etc` (Configuration Files)**

* Tempat **file konfigurasi** sistem & program.
* Contoh: `resolv.conf` (DNS), `logrotate.conf` (pengaturan log).

---

### **`/dev` (Device Files)**

* Folder yang berisi **file perangkat keras**.
* Contoh: `/dev/tty1` (terminal), `/dev/usbmon0` (USB).

---

### **`/proc` (Process Info)**

* Folder semu (pseudo) untuk lihat **proses yang sedang jalan**.
* Contoh: `/proc/uptime` (lihat lama sistem hidup), `/proc/1234` (info proses PID 1234).

---

### **`/var` (Variable Files)**

* File yang **selalu berubah/bertambah**.
* Contoh: `/var/log` (log sistem), `/var/mail` (email), `/var/spool` (antrian print).

---

### **`/tmp` (Temporary Files)**

* Tempat file sementara (hapus otomatis saat reboot).
* Contoh: file hasil download yang belum selesai.

---

### **`/usr` (User Programs)**

* Tempat program tambahan & library.
* `/usr/bin` → program biasa (misalnya `awk`, `scp`).
* `/usr/sbin` → program admin (`sshd`, `cron`).
* `/usr/local` → program hasil **install manual dari source** (misalnya Apache dari source).

---

### **`/home` (Home Directories)**

* Folder pribadi untuk tiap user.
* Contoh: `/home/arya`, `/home/john`.

---

### **`/boot` (Boot Files)**

* File penting buat **booting sistem**.
* Contoh: kernel (`vmlinuz`), `grub`.

---

### **`/lib` (System Libraries)**

* Isi pustaka/library yang dipakai oleh `/bin` & `/sbin`.
* Contoh: `ld-2.11.1.so`.

---

### **`/opt` (Optional Apps)**

* Tempat aplikasi tambahan dari vendor luar.
* Contoh: `/opt/google/chrome`.

---

### **`/mnt` (Mount Point Sementara)**

* Tempat sementara untuk **mount filesystem**.
* Contoh: mount harddisk eksternal di sini.

---

### **`/media` (Removable Media)**

* Tempat **mount otomatis** media eksternal.
* Contoh: `/media/cdrom`, `/media/usb`.

---

### **`/srv` (Service Data)**

* Data khusus untuk **layanan server**.
* Contoh: `/srv/cvs` untuk data CVS server.

---

Intinya:

* `/bin`, `/sbin` → perintah
* `/etc` → konfigurasi
* `/home` → file user
* `/var` → data yang sering berubah
* `/boot` → file booting
* `/dev` & `/proc` → info hardware & proses
* `/mnt` & `/media` → mount storage




