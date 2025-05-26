
# 🛍️ The Bridge – E-commerce Platform

**The Bridge** is a full-stack e-commerce web application built with Flask. It facilitates seamless interactions between buyers and sellers, offering user authentication, product listings, and a streamlined shopping experience.

🔗 **Live Demo**: [https://the-bridge-ekj0.onrender.com](https://the-bridge-ekj0.onrender.com)

## 🚀 Features

- **User Authentication**: Secure login and registration for buyers and sellers.
- **Product Management**: Sellers can list products with images, descriptions, and prices.
- **Shopping Cart**: Buyers can add products to their cart and proceed to checkout.
- **Order Processing**: Manage orders and track purchase history.
- **Responsive Design**: Optimized for desktops, tablets, and mobile devices.

## 🗂️ Project Structure

```
the-bridge/
├── app.py
├── templates/
│   ├── login.html
│   ├── register.html
│   ├── dashboard.html
│   ├── product_list.html
│   └── ...
├── static/
│   ├── css/
│   ├── js/
│   └── images/
├── models.py
├── forms.py
├── requirements.txt
└── README.md
```

## 🛠️ Installation

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/the-bridge.git
cd the-bridge
```

2. **Create and activate a virtual environment**
- **Windows**:
```bash
python -m venv venv
venv\Scripts\activate
```
- **macOS/Linux**:
```bash
python3 -m venv venv
source venv/bin/activate
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

4. **Set environment variables**
Create a `.env` file in the project root and add:
```
FLASK_APP=app.py
FLASK_ENV=development
SECRET_KEY=your-secret-key
```

5. **Initialize the database**
```bash
flask db init
flask db migrate -m "Initial migration."
flask db upgrade
```

6. **Run the application**
```bash
flask run
```
Access the app at `http://localhost:5000`.

## 🌐 Deployment on Render

1. Push your code to GitHub.
2. Create a new Web Service on Render:
   - Build Command: `pip install -r requirements.txt`
   - Start Command: `gunicorn app:app`
   - Environment Variables:
     - FLASK_APP=app.py
     - FLASK_ENV=production
     - SECRET_KEY=your-secret-key
3. Deploy and access your live application at the provided Render URL.

## 🤝 Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.

## 📄 License

This project is licensed under the MIT License.

## 👥 Credits

Developed by **Krishnika**, **Mridula**, and **Poorani**.
