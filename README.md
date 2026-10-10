# Online Food Ordering System (Django)

A restaurant ordering web app built with Django. Customers browse the menu, build a cart, pay and track orders; staff can manage menu items and mark orders as delivered.

## Features
- Landing page, about, hours, directions, contact and privacy pages
- Menu categories: Regular & Sicilian pizza (with toppings), subs, pasta, salads, dinner platters
- User registration, login and logout
- Shopping cart with save and retrieve cart
- Checkout and payment flow
- Order history for users; admin view to mark orders delivered
- Reviews and restaurant listing
- Rich-text content editing in admin via TinyMCE

## Tech Stack
- Python, Django 2.2
- `django-tinymce4-lite`
- HTML / CSS / JavaScript templates, SQLite

## Getting Started
```bash
cd Food-Ordering_Django
python -m venv venv
venv\Scripts\activate          # Windows  (source venv/bin/activate on macOS/Linux)
pip install -r requirements.txt
python manage.py makemigrations
python manage.py migrate
python manage.py createsuperuser   # admin account
python manage.py runserver
```
Open http://127.0.0.1:8000/. Add menu items from the admin at `/admin/`.

See `Food-Ordering_Django/readme.md` for a more detailed setup guide.

> Note: the repository currently contains a committed `venv/` folder; it should be removed and added to `.gitignore`.