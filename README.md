# Pizza-Order-System
A Django-based pizza ordering web application featuring user authentication, menu categories, cart management, and an admin panel. Built with Python, Django, and JavaScript for real-time ordering and tracking.

## Features

- User Authentication
  - Registration and login system for customers
  - Superuser access for admin panel
  - Session management

- Menu Management
  - Multiple pizza categories (Veg Pizza, Non-Veg Pizza, Pizza Combos)
  - Sides and beverages section
  - Dynamic menu updates through admin panel

- Shopping Cart
  - Add/remove items
  - Cart persistence
  - Order summary
  - Checkout process

- Admin Panel
  - Product management
  - Order tracking
  - Delivery status updates
  - Category management

- User Interface
  - Responsive design
  - Intuitive navigation
  - Real-time order updates

## Technology Stack

- Backend: Python, Django
- Frontend: HTML, CSS, JavaScript
- Database: SQLite (default Django DB)
- Session Management: Django Sessions
- Authentication: Django Auth

## Installation

1. Clone the repository
```bash
git clone https://github.com/yourusername/pizza-ordering-system.git
cd pizza-ordering-system
```

2. Create a virtual environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies
```bash
pip install -r requirements.txt
```

4. Run migrations
```bash
python manage.py makemigrations
python manage.py migrate
```

5. Create superuser for admin access
```bash
python manage.py createsuperuser
```

6. Run the development server
```bash
python manage.py runserver
```

## Project Structure

```
pizza_project/
├── orders/                 # Main application directory
│   ├── models.py          # Database models
│   ├── views.py           # View logic
│   ├── urls.py            # URL configurations
│   └── templates/         # HTML templates
├── media/                 # Media files (images, etc.)
├── static/                # Static files (CSS, JS)
└── manage.py             # Django management script
```

## Models

- Category: Pizza categories and descriptions
- UserOrder: Customer order information
- SavedCarts: Persistent shopping cart data
- Various menu item models (Pasta, Salad, Sub, DinnerPlatters)

## Usage

1. Admin Interface:
   - Access `/admin` with superuser credentials
   - Manage products, categories, and orders
   - Track order status

2. Customer Interface:
   - Register/Login through the main interface
   - Browse menu categories
   - Add items to cart
   - Place and track orders
