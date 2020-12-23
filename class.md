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
                "link_video": "https://www.youtube.com/",
                "biaya": "120000",
                "id_class_category": "1",
                "id_status": 4,
                "poster": "1608740267.jpg",
                "updated_at": "2020-12-23T16:17:47.000000Z",
                "created_at": "2020-12-23T16:17:47.000000Z",
                "id_class": 3
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
        "link_video": "-",
        "biaya": "0",
        "id_class_category": "2",
        "id_status": "6"
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
    "totalData": 3,
    "classes": [
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
        },
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
    ```