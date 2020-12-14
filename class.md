# Create Class

* Endpoint: `/api/admin/create-class`
* HTTP Method: `POST`
* Request Header:
    * Accept: `application/json`
* Request Body:
    ```JSON
    {
        "nama": "Kelas Hidroponik",
        "poster": "20200824_123156.jpg",
        "deskripsi": "Kelas ini mengajarkan tentang hidroponik",
        "date_class": "2020-12-19",
        "link_video": "https://www.youtube.com/",
        "biaya": "120000",
        "id_class_category": "1"
    }
    ```
* Response Body:
    ```JSON
    {
        "status": "Success",
        "data": {
            "class": {
                "nama": "Kelas Hidroponik",
                "deskripsi": "Sebuah kelas yang menghadirkan praktisi hidroponik untuk berbagi pengetahuan dan pengalaman selama menekuni hidroponik",
                "date_class": "2020-12-19",
                "link_video": "https://www.youtube.com/",
                "biaya": "120000",
                "id_class_category": "1",
                "poster": "1607955700.jpg",
                "updated_at": "2020-12-14T14:21:40.000000Z",
                "created_at": "2020-12-14T14:21:40.000000Z",
                "id_class": 4
            }
        }
    }
    ```

# Update Class

* Endpoint: `/api/admin/update-class/3`
* HTTP Method: `POST`
* Request Header:
    * Accept: `application/json`
* Request Body:
    ```JSON
    {
        "nama": "Kelas Vertikular",
        "poster": "20200824_184539.jpg",
        "deskripsi": "Kelas ini mengajarkan tentang vertikular",
        "date_class": "2020-12-20",
        "link_video": "-",
        "biaya": "0",
        "id_class_category": "2"
    }
    ```
* Response Body:
    ```JSON
    -
    ```

# Delete Class

* Endpoint: `/api/admin/delete-class/3`
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
                "id_class": 1,
                "nama": "Kelas Hidroponik : Dari Hobi Jadi Bisnis Masa Kini",
                "poster": "IMG-20201202-WA0000.jpg",
                "deskripsi": "Sebuah kelas yang menghadirkan praktisi hidroponik untuk berbagi pengetahuan dan pengalaman selama menekuni hidroponik",
                "date_class": "2020-09-19",
                "link_video": "-",
                "biaya": 0,
                "id_class_category": 1,
                "created_at": "2020-12-14T13:55:57.000000Z",
                "updated_at": "2020-12-14T13:55:57.000000Z"
            },
            {
                "id_class": 2,
                "nama": "Kelas Microgreens 101 : Get to Know More about Microgreens",
                "poster": "IMG-20201202-WA0001.jpg",
                "deskripsi": "Sebuah kelas yang menghadirkan praktisi microgreens untuk berbagi pengetahuan dan pengalaman selama menekuni microgreens",
                "date_class": "2020-09-27",
                "link_video": "-",
                "biaya": 0,
                "id_class_category": 2,
                "created_at": "2020-12-14T13:55:57.000000Z",
                "updated_at": "2020-12-14T13:55:57.000000Z"
            }
        ]
    }
    ```