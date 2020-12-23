# Register Class

* Endpoint: `/api/member/register-class`
* HTTP Method: `POST`
* Request Header:
    * Accept: `application/json`
* Request Body:
    ```JSON
    {
        "id_class": "2",
    }
    ```
* Response Body:
    ```JSON
    {
        "status": "Success",
        "data": {
            "id_member": 2,
            "id_status": 5,
            "id_class": "2",
            "updated_at": "2020-12-11T16:22:03.000000Z",
            "created_at": "2020-12-11T16:22:03.000000Z",
            "id": 2
        }
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
                    "id": 2,
                    "id_member": 2,
                    "id_class": 2,
                    "id_status": 5,
                    "created_at": "2020-12-11T16:22:03.000000Z",
                    "updated_at": "2020-12-11T16:22:03.000000Z"
                }
            ]
        }
    }
    ```  

# Show Detail Registered Class

* Endpoint: `/api/member/show-detail-class/2`
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
    "data": {
        "class": {
            "id_class": 1,
            "nama": "Kelas Hidroponik : Dari Hobi Jadi Bisnis Masa Kini",
            "poster": "IMG-20201202-WA0000.jpg",
            "deskripsi": "Sebuah kelas yang menghadirkan praktisi hidroponik untuk berbagi pengetahuan dan pengalaman selama menekuni hidroponik",
            "link_video": "-",
            "biaya": 0,
            "id_class_category": 1,
            "id_status": 4,
            "created_at": "2020-12-23T15:49:23.000000Z",
            "updated_at": "2020-12-23T15:49:23.000000Z",
            "member_class": [
                {
                    "id": 1,
                    "id_member": 1,
                    "id_class": 1,
                    "id_status": 5,
                    "created_at": "2020-12-23T16:01:08.000000Z",
                    "updated_at": "2020-12-23T16:01:08.000000Z"
                }
            ]
        }
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