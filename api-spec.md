```markdown
# 🔌 API Specification

Dokumentasi lengkap tersedia via Swagger UI saat menjalankan backend di `http://localhost:5000/swagger`.

## Base URL
`http://localhost:5000/api`

## Daftar Endpoint Utama

### 1. Authentication
- **POST** `/Auth/login`: Masuk ke sistem (Return: JWT Token).
- **POST** `/Auth/register`: Pendaftaran mahasiswa baru.

### 2. Rooms (Ruangan)
- **GET** `/Rooms`: Mengambil semua data ruangan.
- **POST** `/Rooms`: Menambah ruangan baru (Admin only).
- **PUT** `/Rooms/{id}`: Update status/data ruangan.

### 3. Bookings (Peminjaman)
- **POST** `/Bookings`: Mengajukan peminjaman.
- **GET** `/Bookings/my-bookings`: Melihat riwayat peminjaman sendiri.
- **PUT** `/Bookings/{id}/status`: Approve/Reject peminjaman (Admin only).