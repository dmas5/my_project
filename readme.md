## Project Structure

```text
Inventory_management_system/
├── app/
│   ├── controllers/
│   │   ├── customerController.js    Handles request for cusomer data
│   │   ├── orderController.js       Handles request for order and order detail
│   │   ├── productController.js     Handles request for product data
│   │   └── supplierController.js    Handles request for supplier data
│   ├── db/
│   │   ├── customer_orderSQL.js     Db interaction with (order,order_detail)
│   │   ├── productSQL.js            Db interaction with table (product)
│   │   └── supplierSQL.js           Db interaction with table (supplier)
│   ├── routes/
│   │   ├── customerRoutes.js        Routes for customer (get,delete)
│   │   ├── orderRoutes.js           Routes for order (get,post,put)
│   │   ├── productRoutes.js         Routes for product (get,post)
│   │   └── supplierRoutes.js        Routes for supplier (get,post,put,delete)
│   ├── services/
│   │   └── sql.js                   Helper function for db interaction
│   └── server.js
├── inventory.sql                    SQL table definitions & insert statements
└── start.js                         Main file
```

