# API Reference

Dokumentasi untuk endpoint-endpoint utama pada API Anda.

---

## POST /v1/bidang

Membuat bidang baru.

### Authentication

Endpoint ini membutuhkan autentikasi Basic Auth.

- **Username:** `{{basic_user}}`
- **Password:** `{{basic_password}}`

### Request

**URL:**  
`POST {{url}}/v1/bidang`

**Headers:**


**Body:**
```json
{
  "kode_lokasi": "KODE2xax",
  "nomor_sertifikat": "SERT789xxwalaweeexx",
  "tanggal_terbit_sertifikat": "2025-07-03T08:53:07+07:00",
  "nib": "NIB123456",
  "nomor_surat_ukur": "SU-001",
  "luas_bidang_hpl": 1000.5,
  "kode_bidang": "BID001",
  "bidang_id": 1,
  "perolehan_id": 2,
  "created_at": "2025-07-03T08:53:07+07:00",
  "created_by": "admin"
}


{
  "status": "00",
  "message": "success",
  "data": {
    "kode_bidang": "BID001",
    "bidang_id": 1,
    "kode_lokasi": "KODE2xax",
    "perolehan_id": 2,
    "nomor_sertifikat": "SERT789xxwalaweeexx",
    "tanggal_terbit_sertifikat": "2025-07-03T08:53:07+07:00",
    "nib": "NIB123456",
    "nomor_surat_ukur": "SU-001",
    "luas_bidang_hpl": 1000.5,
    "created_at": "2025-07-03T08:53:07+07:00",
    "created_by": "admin"
  }
}

{
  "status": "ISTN05",
  "message": "perolehan_id not found",
  "traceId": "73a5504d-77ec-4574-81ad-a28ae52cd666"
}