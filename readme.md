# MaxxiTani Coding Test

## BASE_URL API
https://maxxitani_real-1-x3301871.deta.app/

## LIST ENDPOINT

### Pegawai
| Method | Endpoint | Description |
|:------:|:--------:|-------------|
|GET|`/pegawai`|untuk menampilkan data seluruh data pegawai|
|GET|`/pegawai/{id}`|menampilkan detail dari 1 pegawai tertentu|
|GET|`/pegawai/divisi/{divisi_id} `|menampilkan list pegawai dari divisi tertentu|
|PUT|`/pegawai/{id}`|untuk merubah data pegawai|
|POST|`/pegawai `|untuk menambah data pegawai|
|DELETE|`/pegawai/{id} `|untuk menghapus data pegawai|

### Divisi
| Method | Endpoint | Description |
|:------:|:--------:|-------------|
|GET|`/divisi`|untuk menampilkan seluruh data divisi|
|PUT|`/pegawai/{id}`|untuk merubah data divisi|
|POST|`/divisi `|untuk menambah data divisi|
|DELETE|`/divisi/{id} `|untuk menghapus data divisi|

### Contoh Pemakaian
**Request**\
POST /pegawai/\
Content-Type: application/json
```JSON
{
    "id": 1,
    "nama_pegawai": "Wahyu Bagus Wicaksono",
    "email": "wahyu@mail.com",
    "nomer_hp": "085123456789",
    "alamat": "Jl Malang Selatan",
    "id_divisi": 1
}
```

**Response**\
HTTP/1.1 200 OK\
Content-Type: application/json
```JSON
{
    "message": "Create Pegawai Success",
}

