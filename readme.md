## Project Structure

```text
RESTAPI_POSTGRES/
├── config/
│   ├── db.js                   # Database connection (pool = new Pool).
│   └── db.sql                  # SQL table definitions.
├── controllers/
│   ├── account.controller.js   # Retrieves data on request + error handling.
│   └── auth.controller.js      # Authentication methods (register, login, logout).
├── middlewares/
│   └── auth.middlewares.js     # Authenticates requests by checking JWT tokens
│                               # in HTTP request headers.
├── models/
│   ├── account.model.js        # Account model and toDTO method that returns
│   └── session.model.js        # Session model and toDTO method.
├── repositories/
│   ├── account.repo.js         # Database interaction with the "accounts" table.
│   └── session.repo.js         # Database interaction with the "session_tokens" table.
├── routers/
│   ├── account.router.js       # Routes for authenticated users.
│   └── auth.router.js          # Authentication routes (POST register, GET login).
├── services/
│   └── auth.service.js         # Business logic: password hashing, account creation,
├── index.js                    # Main application file.
└── .env                        # Environment variables: ACCESS_SECRET_KEY,
