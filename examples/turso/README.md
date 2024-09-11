# Turso Example

This example demonstrates how to use Turso with Dumbo to build a simple CRUD API.

## Running the Example

1. Install dependencies:

   ```bash
   composer install
   ```

2. Start the server:

   ```bash
   composer start
   ```

3. Create a new user:

   ```bash
   curl -X POST http://localhost:8000/users \
     -H "Content-Type: application/json" \
     -d '{"name": "John Doe", "email": "john@example.com"}'
   ```

4. Get all users:

   ```bash
   curl http://localhost:8000/users
   ```

5. Get a specific user (replace 1 with the desired user ID):

   ```bash
   curl http://localhost:8000/users/1
   ```

6. Update a user (replace `1` with the desired user ID):

   ```bash
   curl -X PUT http://localhost:8000/users/1 \
     -H "Content-Type: application/json" \
     -d '{"name": "John Updated", "email": "john.updated@example.com"}'
   ```

7. Delete a user (replace `1` with the desired user ID):

   ```bash
   curl -X DELETE http://localhost:8000/users/1
   ```
