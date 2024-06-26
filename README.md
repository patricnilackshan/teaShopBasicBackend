# **Tea Shop Basic Backend**


## **GET** READ all tea data

**Endpoint:** `127.0.0.1:3000/teas`

**Description:** This endpoint retrieves a list of teas. The response is a JSON array containing objects with the keys "id", "name", and "price".

#### **Response:**
``` json
[
    {
        "id": 1,
        "name": "Masala Tea",
        "price": "Rs.100.00"
    },
    {
        "id": 2,
        "name": "Ginger Tea",
        "price": "Rs.150.00"
    },
    {
        "id": 3,
        "name": "Lemon Tea",
        "price": "Rs.200.00"
    }
]
 ```


## **GET** READ specific tea by its ID

**Endpoint:** `127.0.0.1:3000/teas/1`

**Description:** This endpoint retrieves details of a specific tea identified by TeaID. The response will be in JSON format and will include the tea's ID, name, and price.

#### **Response:**
``` json
{
    "id": 1,
    "name": "Masala Tea",
    "price": "Rs.100.00"
}
 ```


## **POST** CREATE new tea data

**Endpoint:** `127.0.0.1:3000/teas/`

**Description:** The POST request to `/teas/` endpoint allows the client to add a new tea with the specified name and price. The request should include a JSON payload with the "name" and "price" fields.

#### **Request Body**
```json
{
    "name"  : "Choco Tea",
    "price" : "Rs.280.00"
}
```

#### **Response** 
``` json
[
    {
        "id": 1,
        "name": "Masala Tea",
        "price": "Rs.100.00"
    },
    {
        "id": 2,
        "name": "Ginger Tea",
        "price": "Rs.150.00"
    },
    {
        "id": 3,
        "name": "Lemon Tea",
        "price": "Rs.200.00"
    },
    {
        "id": 4,
        "name"  : "Choco Tea",
        "price" : "Rs.280.00"
    }
]
 ```


## **PUT** UPDATE tea data

**Endpoint:** `127.0.0.1:3000/teas/4`

**Description:** This endpoint allows you to update a specific tea using the tea's unique identifier.

#### **Request Body**
```json
{
    "name"  : "Milk Tea",
    "price" : "Rs.300.00"
}
```

#### **Response**
``` json
{
    "id": 4,
    "name"  : "Milk Tea",
    "price" : "Rs.300.00"
}
 ```


## **DELETE** DELETE specific tea by its ID

**Endpoint:** `127.0.0.1:3000/teas/1`

**Description:** The endpoint makes an HTTP DELETE request to delete a specific tea item identified by the provided random number.

#### **Response**
``` json
[
    {
        "id": 2,
        "name": "Ginger Tea",
        "price": "Rs.150.00"
    },
    {
        "id": 3,
        "name": "Lemon Tea",
        "price": "Rs.200.00"
    },
    {
        "id": 4,
        "name"  : "Milk Tea",
        "price" : "Rs.300.00"
    }
]
 ```
