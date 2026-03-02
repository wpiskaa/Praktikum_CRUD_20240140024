# User API Specification

## Create User
Endpoint : POST /api/users

Request Body :

```json
{
  "nama" : "Hafiz Kurniawan",
  "usia" : 20
}
```

Response Body (success) :

```json
{
  "data": {
    "id" : "b98e9148-4c32-48f4-aae5-40dc186d3c19",
    "nama": "Hafiz Kurniawan",
    "usia": 20
  }
}
```

Response Body (failed) :

```json
{
  "error": "Invalid input data"
}
```

## Update User
Endpoint : PUT /api/users/{id}

Request Body :

```json
{
  "nama" : "Hafiz Update",
  "usia" : 21
}
```

Response Body (success) :

```json
{
  "data": {
    "id" : "b98e9148-4c32-48f4-aae5-40dc186d3c19",
    "nama": "Hafiz Update",
    "usia": 21
  }
}
```

Response Body (failed) :

```json
{
  "error": "User not found"
}
```

## Get User
Endpoint : GET /api/users

Response Body (success) :

```json
{
  "data": [
    {
      "age": 21,
      "id": "b98e9148-4c32-48f4-aae5-40dc186d3c19",
      "name": "Hafiz Update"
    },
    {
      "age": 25,
      "id": "c2c98f3e-ffcf-4c6f-bb4e-5bc11a667d75",
      "name": "Tiaz Safitri"
    }
  ],
  "status": "success"
}
```

Response Body (failed) :

```json
{
  "error": "User not found"
}
```

## Delete User
Endpoint : DELETE /api/users/{id}

Response Body (success) :

```json
{
  "message": "User deleted successfully"
}
```

Response Body (failed) :

```json
{
  "error": "User not found"
}
```

Screenshot
<img width="2560" height="1528" alt="Screenshot 2026-03-02 114527" src="https://github.com/user-attachments/assets/4d3f6c02-d346-40b7-a498-7b044b259cad" />

Add
<img width="2560" height="1528" alt="image" src="https://github.com/user-attachments/assets/4c67d50e-3b8c-4e5f-b033-b0d493375e0f" />

Edit
<img width="2560" height="1528" alt="Screenshot 2026-03-02 121236" src="https://github.com/user-attachments/assets/2f23cc03-e28d-4682-ab7d-7ca0f814fe58" />

Delete
<img width="2560" height="1528" alt="image" src="https://github.com/user-attachments/assets/995179af-b565-4b35-b316-fc4e1220830e" />

