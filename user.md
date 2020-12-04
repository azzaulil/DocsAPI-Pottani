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
                "poster": "1607083265.jpg",
                "deskripsi": "Sebuah kelas yang menghadirkan praktisi hidroponik untuk berbagi pengetahuan dan pengalaman selama menekuni hidroponik",
                "link_video": "-",
                "biaya": 0,
                "id_status": 4,
                "created_at": "2020-12-02T09:03:21.000000Z",
                "updated_at": "2020-12-02T09:03:21.000000Z"
            }
        }
    }
    ```