# Spring boot with Redis

This project is to showcase spring boot with redis

## Redis For Windows:

https://github.com/microsoftarchive/redis/releases/tag/win-3.2.100

![Alt text](/screenshots/RedisFolderStructure.png?raw=true "Redis Folder Structure")

![Alt text](/screenshots/RedisServer.png?raw=true "Redis Server")

## Redis GUI:

https://github.com/joeferner/redis-commander

**Redis commander installation:**
npm install -g redis-commander

**Run Redis commander:**
redis-commander

![Alt text](/screenshots/RedisCommander.png?raw=true "Redis Commander")

![Alt text](/screenshots/RedisCommanderGUI.png?raw=true "Redis Commander GUI")

## Starting the application

![Alt text](/screenshots/StartApplication.png?raw=true "Start Application")

![Alt text](/screenshots/ApplicationStarted.png?raw=true "Application Started")

## Cache Functionality

![Alt text](/screenshots/CacheFunctionality.png?raw=true "Cache Functionality")

# APIs

Allows you to retrieve, create, update, and delete your products.

## Get Products

- `GET /product.` will return `200 OK` and a list of products created by the user.

```json
[
  {
    "id": 105,
    "name": "Mobile",
    "qty": 2,
    "price": 20000
  },
  {}
]
```

## Get Product

- `GET /product/<product_id>.json` will return `200 OK` and a JSON representation of the specified product.

```json
{
  "id": 105,
  "name": "Mobile",
  "qty": 2,
  "price": 20000
}
```

## Create product

- `POST /product` will create a new product.

```json
{
  "id": 105,
  "name": "Mobile",
  "qty": 2,
  "price": 20000
}
```

This will return `201 Created`, if successful.

## Update product

- `PUT /product/<product_id>.json` will update an existing product.

```json
{
  "id": 105,
  "name": "Mobile",
  "qty": 2,
  "price": 20000
}
```

Will return a `200 OK` response and a JSON representation of the product.

## Delete product

- `DELETE /product/<product_id>` will delete the specified product.

Will return 'Product deleted'
