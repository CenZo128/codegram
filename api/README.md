# API DOCUMENTATION

- Server : **http://localhost:3000**

- SUMMARY: Codegram merupakan aplikasi untuk posting image seperti _Social Media_.

---

## Endpoints

Aplikasi terdiri dari 2 _tables_ : `Users` dan `Postings`

### Users

- GET : /users

  - Request

    - Tidak ada

  - Response

    - `200`

      - ```json
        [
          {
            "id": 1,
            "username": "admin123",
            "email": "admin@mail.com",
            "password": "123",
            "avatar": "https://via.placeholder.com/150",
            "createdAt": "22-11-2021",
            "updatedAt": "22-11-2021"
          }
        ]
        ```

    - `500`

      - ```json
            {
                "message" : "error message",
            }
        ```

- GET : /users/account

- POST : /users

- PUT : /users/:id

- DELETE : /users/:id

### Postings

- GET : /postings

- GET : /postings/details/:id

- GET : /postings/:userId

- POST : /postings

- PUT : /postings/:id

- DELETE : /postings/:id
