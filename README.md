# **Product Listing App**

This project is a **Product Listing App** built using **Node.js**, **Express.js**, and **PostgreSQL**. It provides **CRUD operations** to manage products (create, read, update, delete). Follow the instructions below to set up the project on your local machine.

---

## **Prerequisites**

Make sure you have the following installed on your system:

- **Node.js**: [Install Node.js](https://nodejs.org/)
- **PostgreSQL**: [Install PostgreSQL](https://www.postgresql.org/download/)

---

## **PostgreSQL Database Setup**

1. **Create a PostgreSQL Database:**
   - Open **pgAdmin** or connect to PostgreSQL via the terminal.
   - Run the following SQL command to create the `product_listing` database:
     ```sql
     CREATE DATABASE product_listing;
     ```

2. **Update Database Credentials in `server.js`:**
   - Open the `server.js` file and modify the `Pool` configuration with your PostgreSQL credentials:
     ```javascript
     const pool = new Pool({
       user: 'postgres',            // PostgreSQL username
       host: 'localhost',            // Use 'localhost' for local connections
       database: 'product_listing',  // Database name (replace with your DB name)
       password: 'YourPassword',     // PostgreSQL password
       port: 5432,                   // Default PostgreSQL port
     });
     ```

---

## **Project Setup**

1. **Clone the Repository:**
   In your terminal, run the following command:
   ```bash
   git clone https://github.com/Harshithasagili/Project_Hannah.git

## **Install Dependencies**  
Install the required Node.js packages by running:

```bash
npm install
npm install cross-env --save-dev
npm run install-all
## **Starting the Server**

### **Run the Backend Server**  
Use the following command to start the server on **port 5001**:

```bash
npm start
### **Verify the Server**  
Open your browser and go to:

```bash
http://localhost:5001/products

