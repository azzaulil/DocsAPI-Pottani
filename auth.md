# Login

* Endpoint: `/api/auth/login`
* HTTP Method: `POST`
* Request Header:
    * Accept: `application/json`
* Request Body:
    ```JSON
    {
        "email": "admin@gmail.com",
        "password": "12345678"
    }
    ```
* Response Body:
    ```JSON
    {
        "status": "Success",
        "id_role": 1,
        "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiJ9.eyJhdWQiOiIxIiwianRpIjoiNTc4NmEyOGFmZjA1ZmQzNWQwMDg3MWY4YmE2ZjJiNWE1M2FjOTQ1YmQ1YTA5ZWJlNjg4ZDBmNGNiMmY5YWNmYTE5OTc0OWY4ZjhkNzVmNzYiLCJpYXQiOjE2MDUwNzg0NzcsIm5iZiI6MTYwNTA3ODQ3NywiZXhwIjoxNjM2NjE0NDc3LCJzdWIiOiIxIiwic2NvcGVzIjpbXX0.UfbwkK3venNcSAPb5IKAkttNIFVKXmlLH1NEL7-eONk-nnomCRN3Ht72pkjAtpflQ7gDe4eH75n0DfqhmLl2h5sweXjhsu3y4-je4jN6LhN6xPCrbkYtcx3dnxGqruBZ4PComJxAl7nMPwsI3JaUgaAD60NYx5VwWpZFp4d7tUS5tsl9RTsGG1pRG7FWlmAtBzHEX_nNAhg943gPFryinlNJVGhfLvWRacbzQFpbkdgM2Khh4A2twhY_uiZqTy7D4A-eT6pdNa7S40DrDFJPqDkGB6bwC7KUYJc2pJ3JDFrWkTSFeROK56qHo28sxE_3UWRBqfMNijncVfRyua9gYgWxsMB3qABkAscc25LbIjfrsdHZYUL9ztHEI5D-OoeuEViEjUrYrH_b2brfgFWCdLzbmqMGB5sBG90uir04HVhMERyWeTDNxOZyofpSlOTggKfYJYaIUs7vpj2OYe_5IPNxIIEMh_wKGgLb6vIcNQMSfFyQHfUVWb3dleKHFgV10d_zLDq9uyOVcrYMItC3Go2NJom28SEHOC9STjQ7-yHsT6dN41F4lg4-j1L9cpII3beJIRIhxjgE0AGw-_oZiNLTpkPXbqFW5GNjBdjUaVHsWtSu0O4uH-TO3C-UHPJ3cZYx6vNxGgF3KF3zW3MxSQI7EAM4J_HwJqzz2c9gVI4",
        "role": "Admin"
    }
    ```


# Register

* Endpoint: `/api/auth/register`
* HTTP Method: `POST`
* Request Header:
    * Accept: `application/json`
* Request Body:
    ```JSON
    {
        "email": "test@mail.com",
        "password": "12345678",
        "password_confirmation": "12345678",
        "nama_lengkap": "Ini Testing",
        "alamat": "Jogja",
        "jenis_kelamin": "L",
        "usia": "21",
        "telepon": "0846272634"
    }
    ```
* Response Body:
    ```JSON
    {
        "status": "Created",
        "message": "Successfully registered as Member!"
    }
    ```
