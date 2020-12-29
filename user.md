# Show All Class

* Endpoint: `/api/auth/show-all-class`
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
            "kelas yang buka": [
                {
                    "id_class": 1,
                    "nama": "Kelas Hidroponik : Dari Hobi Jadi Bisnis Masa Kini",
                    "poster": "IMG-20201202-WA0000.jpg",
                    "deskripsi": "Sebuah kelas yang menghadirkan praktisi hidroponik untuk berbagi pengetahuan dan pengalaman selama menekuni hidroponik",
                    "link_video": "-",
                    "biaya": 0,
                    "id_class_category": 1,
                    "id_status": 4,
                    "created_at": "2020-12-23T15:49:23.000000Z",
                    "updated_at": "2020-12-23T15:49:23.000000Z"
                }
            ],
            "kelas yang tutup": [
                {
                    "id_class": 2,
                    "nama": "Kelas Microgreens 101 : Get to Know More about Microgreens",
                    "poster": "IMG-20201202-WA0001.jpg",
                    "deskripsi": "Sebuah kelas yang menghadirkan praktisi microgreens untuk berbagi pengetahuan dan pengalaman selama menekuni microgreens",
                    "link_video": "-",
                    "biaya": 0,
                    "id_class_category": 2,
                    "id_status": 6,
                    "created_at": "2020-12-23T15:49:23.000000Z",
                    "updated_at": "2020-12-23T15:49:23.000000Z"
                },
                {
                    "id_class": 3,
                    "nama": "Kelas Vertikular",
                    "poster": "1608740532.jpg",
                    "deskripsi": "Sebuah kelas yang menghadirkan praktisi hidroponik untuk berbagi pengetahuan dan pengalaman selama menekuni hidroponik",
                    "link_video": "-",
                    "biaya": 0,
                    "id_class_category": 2,
                    "id_status": 6,
                    "created_at": "2020-12-23T16:17:47.000000Z",
                    "updated_at": "2020-12-23T16:22:12.000000Z"
                }
            ]
        }
    }
    ```

# Show Detail Class

* Endpoint: `/api/auth/show-detail-class/1`
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
                "updated_at": "2020-12-23T15:49:23.000000Z"
            }
        }
    }
    ```