**About**
Ini adalah klien / server multithreaded ChatServer berbasis konsol yang menggunakan pemrograman Java Socket.
Server mendengarkan permintaan koneksi dari klien di seluruh jaringan atau bahkan dari mesin yang sama. Klien tahu bagaimana menghubungkan ke server melalui alamat IP dan nomor port. 
Setelah terhubung ke server, klien dapat memilih nama penggunanya di ruang obrolan. Klien mengirim pesan, pesan tersebut dikirim ke server menggunakan ObjectOutputStream di java. 
Setelah menerima pesan dari klien, server menyiarkan pesan jika itu bukan pesan pribadi. Dan jika itu adalah pesan pribadi yang dideteksi menggunakan '@' diikuti dengan nama pengguna yang valid, maka kirimkan pesan hanya ke pengguna tersebut. 
Serialisasi objek Java untuk mentransfer pesan.

**Instruksi**
**Client**

Untuk memulai Client dalam mode konsol, gunakan salah satu dari perintah berikut ini :
 1. java Client
 2. java Client username
 3. java Client username portNumber
 4. java Client username portNumber serverAddress

Pada prompt konsol :
Jika portNumber tidak ditentukan 1500 digunakan
Jika serverAddress tidak ditentukan, "localHost" digunakan
Jika nama pengguna tidak ditentukan, "Anonymous" digunakan

**Server**

Untuk dijalankan sebagai aplikasi konsol :
 1. java Server
 2. java Server portNumber
Jika portNumber tidak ditentukan 1500 digunakan

**Chat**

Saat berada di konsol Client:
1. Ketikkan pesan untuk mengirim siaran ke semua klien aktif
2. Ketik '@username<space>yourmessage' tanpa tanda kutip untuk mengirim pesan ke klien yang diinginkan
3. Ketik 'WHOISIN' tanpa tanda kutip untuk melihat daftar klien aktif
4. Ketik 'LOGOUT' tanpa tanda kutip ke logoff dari server
