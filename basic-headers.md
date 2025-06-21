# Header Dasar Email

## Header Wajib (Mandatory Headers)

### From Header
Header `From` adalah header wajib yang mengidentifikasi pengirim email.

**Format:**
```
From: "Nama Pengirim" <email@domain.com>
From: email@domain.com
```

**Contoh:**
```
From: "John Doe" <john.doe@company.com>
From: noreply@bank.com
```

**Keamanan:**
- Mudah dipalsukan (spoofed)
- Tidak boleh diandalkan untuk otentikasi
- Perlu verifikasi tambahan melalui SPF/DKIM

### To Header
Header `To` mengidentifikasi penerima utama email.

**Format:**
```
To: "Nama Penerima" <email@domain.com>
To: email1@domain.com, email2@domain.com
```

**Contoh:**
```
To: "Jane Smith" <jane.smith@company.com>
To: admin@company.com, support@company.com
```

### Subject Header
Header `Subject` berisi judul atau topik email.

**Format:**
```
Subject: Judul Email
```

**Contoh:**
```
Subject: Laporan Bulanan Juli 2024
Subject: [URGENT] Password Reset Required
```

**Keamanan:**
- Sering digunakan dalam phishing untuk memancing respons
- Bisa mengandung karakter berbahaya atau encoding yang mencurigakan

### Date Header
Header `Date` menunjukkan waktu pengiriman email.

**Format:**
```
Date: Day, DD Mon YYYY HH:MM:SS +ZZZZ
```

**Contoh:**
```
Date: Thu, 25 Jul 2024 10:30:00 +0700
Date: Mon, 22 Jul 2024 15:45:30 -0500
```

**Keamanan:**
- Bisa dipalsukan untuk menyembunyikan waktu pengiriman asli
- Berguna untuk deteksi email yang terlalu lama dalam transit

## Header Opsional (Optional Headers)

### Message-ID Header
Header `Message-ID` adalah identifier unik untuk setiap email.

**Format:**
```
Message-ID: <unique-string@domain.com>
```

**Contoh:**
```
Message-ID: <20240725103000.12345@company.com>
Message-ID: <CA+abc123def456@mail.gmail.com>
```

**Keamanan:**
- Membantu melacak email dalam sistem
- Mencegah duplikasi email
- Berguna untuk threading dan grouping

### MIME-Version Header
Header `MIME-Version` menunjukkan versi MIME yang digunakan.

**Format:**
```
MIME-Version: 1.0
```

**Keamanan:**
- Versi yang tidak standar bisa menandakan email berbahaya
- MIME encoding bisa digunakan untuk menyembunyikan konten berbahaya

### Content-Type Header
Header `Content-Type` menentukan tipe konten email.

**Format:**
```
Content-Type: type/subtype; charset=encoding
```

**Contoh:**
```
Content-Type: text/plain; charset=UTF-8
Content-Type: text/html; charset=ISO-8859-1
Content-Type: multipart/mixed; boundary="boundary-string"
```

**Keamanan:**
- HTML content bisa mengandung script berbahaya
- Attachments dengan tipe yang salah bisa mengecoh sistem keamanan 