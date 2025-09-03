# tugas3
# Cobasa

API sederhana untuk manajemen data film dan sutradara menggunakan Express.js.

## Fitur

- Melihat daftar semua film (`GET /movies`)
- Melihat detail film berdasarkan ID (`GET /movies/:id`)
- Melihat detail film berdasarkan judul (`GET /movies/title/:title`)
- Menambah film baru (`POST /movies`)
- Melihat daftar semua sutradara (`GET /directors`)
- Melihat detail sutradara berdasarkan ID (`GET /directors/:id`)
- Menambah sutradara baru (`POST /directors`)
- Mengubah data sutradara (`PUT /directors/:id`)
- Menghapus sutradara (`DELETE /directors/:id`)


## Menjalankan Server

```sh
node server.js
```
atau dengan nodemon (untuk development):
```sh
npx nodemon server.js
```

Server akan berjalan di [http://localhost:3000](http://localhost:3000).

## Contoh Request

- **GET semua film:**  
  `GET /movies`

- **GET film by ID:**  
  `GET /movies/1`

- **GET film by title:**  
  `GET /movies/title/Inception`

- **POST film baru:**  
  `POST /movies`  
  Body (JSON):
  ```json
  {
    "title": "Tenet",
    "director": "Christopher Nolan",
    "year": 2020
  }
  ```

- **GET semua sutradara:**  
  `GET /directors`

- **GET sutradara by ID:**  
  `GET /directors/1`

- **POST sutradara baru:**  
  `POST /directors`  
  Body (JSON):
  ```json
  {
    "name": "Denis Villeneuve",
    "year": 2021
  }
  ```

- **PUT update sutradara:**  
  `PUT /directors/1`  
  Body (JSON):
  ```json
  {
    "name": "Christopher Nolan",
    "year": 2022
  }
  ```

- **DELETE sutradara:**  
  `DELETE /directors/1`

## Lisensi

ISC
