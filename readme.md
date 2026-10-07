## Project Structure

```text
Inventory_management_system/
├── App/
│   ├── Controllers/
│   │   ├── customerController.js
│   │   ├── orderController.js
│   │   ├── productController.js
│   │   └── supplierController.js
│   ├── db/
│   │   ├── customer_orderSQL.js      Db interaction with order and order details table
│   │   ├── productSQL.js             Db interaction with product table
│   │   └── supplierSQL.js            Db interaction with supplier table
│   ├── routes/
│   │   ├── customerRoutes.js         Routes for customer (get)
│   │   ├── orderRoutes.js            Routes for order (get,post,put)
│   │   ├── productRoutes.js          Routes for product (get)
│   │   └── supplierRoutes.js         Routes for supplier (get,post,put)
│   └── services/
│       └── sql.js                    Helper function for db interaction
├── .env
├── Inventory.sql                     SQL table definitions
└── Start.js                          Main file
```

