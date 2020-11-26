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