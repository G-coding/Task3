🍴 RESTAURANT DASHBOARD

    A simple microservices-based restaurant management dashboard built with React (frontend) and Django REST Framework (backend).
    The dashboard allows managing Menu Items, Orders, Reservations, and Inventory in a single UI.

🚀 FEATURES

    1. Menu Management — View restaurant menu items with name, description, and price.
    2. Orders Management — View customer orders.
    3. Reservations — View table reservations with customer details.
    4. Inventory — Track available items and their quantities.
    5. Microservices Architecture — Each module (Menu, Orders, Reservations, Inventory) is powered by its own Django REST API.
    6. React Frontend — Clean, modular UI with navigation.

🛠️ TECH STACK

    Frontend: React, React Router
    Backend: Django + Django REST Framework (microservices)
    Database: MySQL

📂 Project Structure

    ```bash
    Task3/
    │
    ├── backend/
    │   ├── menu_service/
    │   ├── order_service/
    │   ├── reservation_service/
    │   └── inventory_service/
    │
    ├── frontend/  (React app)
    |   └── restaurant-ui
    |       ├── src/
    |       │   ├── components/
    |       │   │   ├── MenuItems.js
    |       │   │   ├── Orders.js
    |       │   │   ├── Reservations.js
    |       │   │   └── Inventory.js
    |       │   └── App.js
    |       └── package.json
    │
    └── README.md

⚙️ Installation
    
    1. Clone Repository
        git clone https://github.com/G-coding/Task3.git
    2. Backend Setup (Django Services)
        Each microservice (menu, orders, reservations, inventory) runs separately.
        Inside each service folder:
            pip install django djangorestframework mysqlclient
            pip install django-cors-headers
            python manage.py makemigrations
            python manage.py migrate
            python manage.py runserver <port>
        Example:
            Menu Service → 127.0.0.1:8001
            Orders Service → 127.0.0.1:8002
            Reservation Service → 127.0.0.1:8003
            Inventory Service → 127.0.0.1:8004
    3. Frontend Setup (React)
        Go to the frontend folder:
            cd frontend
            cd restaurant-ui
            npm install
            npm start
        The app will run on:
            http://localhost:3000

🔗 API Endpoints

    Menu Service -> http://127.0.0.1:8001/api/menu/
    Orders Service -> To get order id -> http://127.0.0.1:8002/api/order/
                      To order items from menu -> http://127.0.0.1:8002/api/order_item/
    Reservations Service -> http://127.0.0.1:8003/api/reservation/
    Inventory Service -> http://127.0.0.1:8004/api/inventory/

📸 Screenshots

    1. Dashboard Navigation
    <img width="1280" height="701" alt="Screenshot 2025-08-24 at 7 18 42 AM" src="https://github.com/user-attachments/assets/bda1bff4-f5ba-4dfe-bff7-ef83d6453d53" />
    2. Menu List
    <img width="1276" height="702" alt="Screenshot 2025-08-24 at 7 19 09 AM" src="https://github.com/user-attachments/assets/e4736376-91f9-4515-ae1f-a8bebe017f05" />
    3. Orders List
    <img width="1280" height="702" alt="Screenshot 2025-08-24 at 7 19 26 AM" src="https://github.com/user-attachments/assets/da3ed42a-9187-464a-977d-4f67973b5de2" />
    4. Reservations
    <img width="1279" height="702" alt="Screenshot 2025-08-24 at 7 19 41 AM" src="https://github.com/user-attachments/assets/cc953021-420d-4ece-aaa5-b21fc15aeeb5" />
    5. Inventory
    <img width="1280" height="702" alt="Screenshot 2025-08-24 at 7 19 55 AM" src="https://github.com/user-attachments/assets/e204a759-abc4-4f0c-b152-26e1c3fbe7e3" />

👩‍💻 Author: Developed by Geetika Agarwal as part of an internship project.

