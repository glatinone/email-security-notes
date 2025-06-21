# Email Headers: Panduan Lengkap

## Pengantar Email Headers

Email headers adalah bagian metadata dari pesan email yang berisi informasi penting tentang perjalanan email dari pengirim ke penerima. Headers ini memainkan peran kritis dalam keamanan email, troubleshooting, dan audit trail.

### Komponen Dasar Email Header

Setiap email terdiri dari dua bagian utama:
1. **Headers** - Metadata dan informasi routing
2. **Body** - Konten pesan yang sebenarnya

Headers ditulis dalam format RFC 5322 dan berisi informasi seperti:
- Alamat pengirim dan penerima
- Timestamp pengiriman
- Server yang terlibat dalam routing
- Informasi keamanan dan otentikasi
- Metadata teknis lainnya

### Struktur Hierarkis Email Headers

Email headers mengikuti struktur hierarkis yang jelas:
```
From: sender@domain.com
To: recipient@domain.com
Subject: Email Subject
Date: Thu, 25 Jul 2024 10:30:00 +0700
Message-ID: <unique-identifier@domain.com>
MIME-Version: 1.0
Content-Type: text/plain; charset=UTF-8
```

### Pentingnya Email Headers dalam Keamanan

Email headers sangat penting dalam keamanan karena:
- Memungkinkan deteksi spoofing dan phishing
- Menyediakan audit trail lengkap
- Mendukung protokol keamanan seperti SPF, DKIM, dan DMARC
- Membantu dalam investigasi keamanan
- Memungkinkan filtering dan blocking berdasarkan kriteria tertentu 