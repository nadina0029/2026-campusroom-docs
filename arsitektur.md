# 🏗️ Arsitektur Sistem

## 1. Tech Stack
| Komponen | Teknologi | Keterangan |
| --- | --- | --- |
| **Frontend** | React.js + TypeScript | Antarmuka pengguna (Web) |
| **Backend** | ASP.NET Core Web API | Logika bisnis & REST API |
| **Database** | SQL Server | Penyimpanan data relasional |

## 2. Diagram Alur Data (Simplified)
```mermaid
graph LR
    User[Mahasiswa] -->|Request Booking| Frontend
    Frontend -->|API Call| Backend
    Backend -->|Query/Save| Database
    Database -->|Result| Backend
    Backend -->|Response JSON| Frontend
    Frontend -->|Show Notification| User