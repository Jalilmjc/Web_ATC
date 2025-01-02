# ATC Management System
The ATC Management System is a web-based application designed for Altaf Trading Company (ATC) to manage its business operations efficiently. This system offers customer, product, and order management, along with advanced data science features such as sales forecasting, customer segmentation, and recommendation systems. The platform is built using Python (Flask), MySQL, and frontend technologies like HTML, CSS, and JavaScript, with deployment capabilities for real-time access.
Step 1: Clone the Repository
To start using this project, you need to clone it to your local machine.
git clone https://github.com/Jalilmjc/Web_ATC.git
cd Web_ATC
Step 2: Install the Required Dependencies
Ensure you have Python and pip installed on your system.
Install the required Python packages using the requirements.txt file:
pip install -r requirements.txt
Step 3: Set Up the Database
Install MySQL on your machine.
Create a database named atc.
Run the SQL script (if provided) to set up the tables:
SOURCE /path/to/your/sql_script.sql;
Update the database connection details in backend/server.py if necessary:
conn = pymysql.connect(
    host="localhost",
    user="root",
    password="",
    database="atc",
    charset="utf8mb4"
)
Step 4: Run the Backend
Navigate to the backend folder.
Start the Flask server:
python server.py
Verify the server is running by visiting:
http://127.0.0.1:5001/
You should see the message:
Welcome! Backend is working.
Step 5: Run the Frontend
Open the index.html file in a browser.
Use the interface to:
Manage customers
Manage products
Create orders
View analytics dashboards
Step 6: Test Backend Features
You can test the backend API endpoints using tools like Postman or curl.

Example API Request: Add a Customer
curl -X POST http://127.0.0.1:5001/customers \
-H "Content-Type: application/json" \
-d '{"firstName": "Muhammad", "lastName": "Jalil", "email": "jalilaridian@gmail.com"}'
