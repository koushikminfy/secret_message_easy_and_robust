

# Secret Message Service 

---

# (Basic)

##  Getting Started


### 1. Install Dependencies

```bash
bun install
```

### 2. Run the Server

```bash
bun start
```

---

##  API Endpoints

###  POST `/messages` – Create a New Message

**Request Body:**

```json
{
  "message": "The eagle has landed and is hungry."
}
```
![118](https://github.com/user-attachments/assets/7ee33b4c-de78-4dd3-9e07-1b5fc720f1bf)

**Success Response (201 Created):**

---

### POST `/messages` – Validation Failure

**Request Body:**

```json
{
  "message": "Too short"
}

```

![119](https://github.com/user-attachments/assets/e005cbe9-f0ae-445b-b6b7-9549fa9253f2)

**Response (400 Bad Request):**

---

###  GET `/messages/:id` – Retrieve Message by ID

**Example:**

```http
GET http://localhost:3000/messages/0
```

![120](https://github.com/user-attachments/assets/eace1cdc-03ea-4c3f-a861-84bc7800264d)




---





---
## Robust
##  Project Structure 

```
secret-message-robust/
├── src/
│   ├── controllers/
│   │   └── messageController.js
│   ├── middleware/
│   │   ├── errorHandler.js
│   │   └── logger.js
│   ├── routes/
│   │   └── messageRoutes.js
│   ├── utils/
│   │   └── inMemoryDb.js
│   └── index.js
├── package.json
```

---

##  Step-by-Step Setup

### 1. Initialize Project


```markdown
#  Secret Message Service (Robust)
---


##  Getting Started

### 1. Install dependencies

```bash
bun install
````

### 2. Start the server

```bash
bun start
```

---

##  API Endpoints

###  `POST /` — Create a message
* `POST http://localhost:3000/api/v1/messages`
**Body:**

```json
{
  "message": "This is a valid message."
}
```

**Response:**
![1000](https://github.com/user-attachments/assets/9a933a87-c78d-44fd-ab2e-0bd8fbb02028)



###  `GET /` — Get all messages
* `GET http://localhost:3000/api/v1/messages`
**Response:**
![1001](https://github.com/user-attachments/assets/f42ab409-be34-4729-8d14-ae4c6ac77d39)



###  `GET /:id` — Get message by ID
* `GET http://localhost:3000/api/v1/messages/:id`
**Response :**

![1003](https://github.com/user-attachments/assets/138a738a-5878-49db-862a-f13cf29ad077)



###  `DELETE /:id` — Delete message by ID
* `DELETE http://localhost:3000/api/v1/messages/:id`
**Response:**

![1004](https://github.com/user-attachments/assets/5d67216a-9556-41f7-a898-e37321035542)





---

