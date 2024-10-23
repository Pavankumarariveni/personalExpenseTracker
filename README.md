# Personal Expense Tracker API

## Setup Instructions
    1. Clone the repository.
    2. Run `npm install` to install dependencies.
    3. Run `node server.js` to start the server.

## API Endpoints

### POST /transactions
- **Request Body**: `{ "type": "income/expense", "category": <category_id>, "amount": <number>, "date": "YYYY-MM-DD", "description": "string" }`
- **Response**: `{ "id": <transaction_id>, ... }`

### GET /transactions
- **Response**: Array of transaction objects.

### GET /transactions/:id
- **Response**: Transaction object by ID.

### PUT /transactions/:id
- **Request Body**: Same as POST.
- **Response**: `{ "UpdatedId": <transaction_id>}`

### DELETE /transactions/:id
- **Response**: `{ "DeletedId": <transaction_id>}`

### GET /summary
- **Response**: Summary of transactions.

## Postman Examples
### POST /transactions
https://1drv.ms/i/c/ceacdf473fcc0ade/EROLVPFokQZOplWSxt8Q2jgBawGIC9rRY6HmSd8q8UNyuw?e=OdPsgY

### GET /transactions
https://1drv.ms/i/c/ceacdf473fcc0ade/EW_fKvDKD3VKnuaTOuV7Yu8BmwDiEAkoKZxkgQI26Vfpeg?e=TuXtTY

### GET /transactions/:id
https://1drv.ms/i/c/ceacdf473fcc0ade/EVM7LYTko4hHn-ly9YjPQ80BPAFGV479ixExiild_qC5Pw?e=Giksko

### PUT /transactions/:id
https://1drv.ms/i/c/ceacdf473fcc0ade/EYE1KEU4LiFDmElvA6mJCmsBtixUGY9y4iGIPMB2zRPMEQ?e=NLqese

### DELETE /transactions/:id
https://1drv.ms/i/c/ceacdf473fcc0ade/Eb1uplI9zdlLlEoWNy-XLecBmSk4yB7hHwfj1dgeqTzsqQ?e=ebqMvb