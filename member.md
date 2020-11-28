# Show All Class

* Endpoint: `/api/member/show-all-class`
* HTTP Method: `GET`
* Request Header:
    * Accept: `application/json`
* Request Body:
    ```JSON
    -
    ```
* Response Body:
    ```JSON
    {
    "status": "Success",
    "size": 1,
    "data": {
        "class": [
            {
                "id_class": 1,
                "nama": "Kelas Hidroponik",
                "poster": "20200824_123156.jpg",
                "deskripsi": "Kelas ini mengajarkan tentang hidroponik",
                "link_video": "https://www.youtube.com/",
                "biaya": 150000,
                "id_status": 4,
                "created_at": "2020-11-28T10:07:28.000000Z",
                "updated_at": "2020-11-28T10:07:28.000000Z"
            }
        ]
    }
}
    ```

# Register Class

* Endpoint: `/api/member/register-class`
* HTTP Method: `POST`
* Request Header:
    * Accept: `application/json`
* Request Body:
    ```JSON
    {
        "id_class": "1",
    }
    ```
* Response Body:
    ```JSON
    {
        "id_member": 1,
        "id_status": 5,
        "id_class": "1",
        "updated_at": "2020-11-26T07:14:35.000000Z",
        "created_at": "2020-11-26T07:14:35.000000Z",
        "id": 2
    }
    ```

# Show Registered Class

* Endpoint: `/api/member/show-registered-class`
* HTTP Method: `GET`
* Request Header:
    * Accept: `application/json`
* Request Body:
    ```JSON
    -
    ```
* Response Body:
    ```JSON
{
    "status": "Success",
    "size": 1,
    "data": {
        "class": [
            {
                "id": 1,
                "id_member": 1,
                "id_class": 1,
                "id_status": 5,
                "created_at": "2020-11-26T03:47:19.000000Z",
                "updated_at": "2020-11-26T03:47:19.000000Z"
            }
        ]
    }
}
    ```    

# Show Profile

* Endpoint: `/api/member/show-profile`
* HTTP Method: `GET`
* Request Header:
    * Accept: `application/json`
* Request Body:
    ```JSON
    -
    ```
* Response Body:
    ```JSON
{
    "status": "Success",
    "size": 1,
    "data": {
        "member": [
            {
                "id_users": 2,
                "id_role": 2,
                "is_active": 1,
                "email": "member@gmail.com",
                "created_at": "2020-11-28T10:07:27.000000Z",
                "updated_at": "2020-11-28T10:07:27.000000Z",
                "member": {
                    "id_member": 1,
                    "id_users": 2,
                    "nama_lengkap": "Member Tes",
                    "alamat": "Tes Alamat",
                    "usia": "20 Tahun",
                    "telepon": "088",
                    "foto_profil": null,
                    "jenis_kelamin": "L",
                    "created_at": "2020-11-28T10:07:28.000000Z",
                    "updated_at": "2020-11-28T10:07:28.000000Z"
                }
            }
        ]
    }
}
    ```    

# Update Profile

* Endpoint: `/api/member/update-profile`
* HTTP Method: `POST`
* Request Header:
    * Accept: `application/json`
* Request Body:
    ```JSON
    {
        "nama_lengkap": "Member Pottani",
        "jenis_kelamin": "P",
        "telepon": "0812356756",
    }
    ```
* Response Body:
    ```JSON
    {
        "id_member": 1,
        "id_users": 2,
        "nama_lengkap": "Member Pottani",
        "alamat": "Tes Alamat",
        "usia": "20 Tahun",
        "telepon": "0895396616984",
        "foto_profil": null,
        "jenis_kelamin": "P",
        "created_at": "2020-11-28T10:07:28.000000Z",
        "updated_at": "2020-11-28T11:03:54.000000Z"
    }
    ```