# Mini REST API with Express.js

This is a simple REST API built with Node.js and Express.js. It manages an in-memory list of items.

## 📦 Installation

```bash
git clone <repo-url>
cd mini-express-api
npm install
```

## ▶️ Running the Server

```bash
npm start
```

Server runs at `http://localhost:3000`

## 🛠 API Endpoints

### 1. GET /
- Returns: `"Hello, World!"`

### 2. GET /items
- Returns all items

### 3. GET /items/:id
- Returns a single item

### 4. POST /items
- Body: `{ "name": "Item 1", "description": "Test desc" }`

### 5. PUT /items/:id
- Updates item by ID

### 6. DELETE /items/:id
- Deletes item by ID

## 🧪 Example Requests (Postman)

### Add Item
```
POST http://localhost:3000/items
Body:
{
  "name": "Phone",
  "description": "An Android device"
}
```

### Get All Items
```
GET http://localhost:3000/items
```

### Get Item by ID
```
GET http://localhost:3000/items/<id>
```

### Update Item
```
PUT http://localhost:3000/items/<id>
Body:
{
  "name": "Updated Phone",
  "description": "Updated description"
}
```

### Delete Item
```
DELETE http://localhost:3000/items/<id>
```

## ❗ Error Responses

- 400: Missing fields
- 404: Item or route not found
- 500: Internal server error