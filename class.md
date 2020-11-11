# Create Class

* Endpoint: `/api/admin/create-class`
* HTTP Method: `GET`
* Request Header:
    * Accept: `application/json`
* Request Body:
    ```JSON
    {
        "nama": "Kelas Hidroponik",
        "poster": "20200824_123156.jpg",
        "deskripsi": "Kelas ini mengajarkan tentang hidroponik",
        "link_video": "https://www.youtube.com/",
        "biaya": "150000"
    }
    ```
* Response Body:
    ```JSON
    {
        "status": "Success",
        "data": {
            "class": {
                "nama": "Kelas Hidroponik",
                "deskripsi": "Kelas ini mengajarkan tentang hidroponik",
                "link_video": "https://www.youtube.com/",
                "biaya": "150000",
                "poster": "1605105680.jpg",
                "updated_at": "2020-11-11T14:41:20.000000Z",
                "created_at": "2020-11-11T14:41:20.000000Z",
                "id": 3
            }
        }
    }
    ```

# Update Class

* Endpoint: `/api/admin/update-class/2`
* HTTP Method: `POST`
* Request Header:
    * Accept: `application/json`
* Request Body:
    ```JSON
    {
        "nama": "Kelas Vertikular",
        "poster": "20200824_184539.jpg",
        "deskripsi": "Kelas ini mengajarkan tentang vertikular",
        "link_video": "https://www.youtube.com/",
        "biaya": "120000"
    }
    ```
* Response Body:
    ```JSON
    -
    ```

# Delete Class

* Endpoint: `/api/admin/delete-class/1`
* HTTP Method: `DELETE`
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
        "message": "deleted success"
    }
    ```

# Show Class

* Endpoint: `/api/admin/show-class`
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
        "message": "Success",
        "totalData": 2,
        "classes": [
            {
                "id": 2,
                "nama": "Kelas Vertikular",
                "poster": "1605107188.jpg",
                "deskripsi": "Kelas ini mengajarkan tentang vertikular",
                "link_video": "https://www.youtube.com/",
                "biaya": 120000,
                "created_at": "2020-11-11T14:40:25.000000Z",
                "updated_at": "2020-11-11T15:06:28.000000Z"
            },
            {
                "id": 3,
                "nama": "Kelas Hidroponik",
                "poster": "1605105680.jpg",
                "deskripsi": "Kelas ini mengajarkan tentang hidroponik",
                "link_video": "https://www.youtube.com/",
                "biaya": 150000,
                "created_at": "2020-11-11T14:41:20.000000Z",
                "updated_at": "2020-11-11T14:41:20.000000Z"
            }
        ]
    }
    ```