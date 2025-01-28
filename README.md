# Finance Tracker App

## **Project Summary**

The **Finance Tracker App** is a full-stack application designed to demonstrate skills in building and deploying a robust, intuitive solution for tracking income, expenses, and budgets. It provides users with an easy-to-use interface and secure backend functionality.

---

## **Tech Stack**

### **Frontend**

- **Framework**: React with Vite for fast development.
- **Styling**: TailwindCSS for a modern, responsive design.
- **State Management**: Redux Toolkit for efficient and scalable global state handling.
- **Libraries**:
  - **Axios**: For API requests to the backend.
  - **React Router Dom**: For client-side routing between pages.
  - **React-Chartjs-2** (or **Recharts**) for interactive data visualization.

### **Backend**

- **Framework**: Flask with JWT for lightweight and efficient API handling.
- **Database**: PostgreSQL for relational data storage.
- **Libraries**:
  - **Flask-RESTful**: For building RESTful APIs.
  - **Flask-JWT-Extended**: For secure user authentication and token management.
  - **SQLAlchemy**: For database ORM.
  - **Marshmallow**: For data serialization and validation.
  - **Flask-CORS**: To handle cross-origin requests between frontend and backend.

### **Hosting**

- **Frontend**: Netlify for hosting the React app.
- **Backend**: AWS (EC2 for the Flask app and RDS for the PostgreSQL database).

---

## **Project Structure**

### **Frontend**

Folder: `finance-tracker-frontend/`

```
src/
    ├── components/       # Reusable UI components
    ├── pages/            # Page components (e.g., Dashboard, Login)
    ├── store/            # Redux slices and store
    ├── App.jsx           # Main app file
    ├── index.css         # TailwindCSS styles
    └── main.jsx          # App entry point
```

### **Backend**

Folder: `finance-tracker-backend/`

```
app/
    ├── __init__.py       # Flask app factory
    ├── models.py         # SQLAlchemy models
    ├── routes.py         # API endpoints
    ├── schemas.py        # Marshmallow schemas
    ├── auth.py           # JWT authentication logic
    └── config.py         # App configuration (e.g., database URI)
requirements.txt          # Backend dependencies
run.py                    # Flask app runner
```

---

## **Planned Features**

### **User Authentication**

- Users can register, log in, and log out securely.
- Authentication is managed via **JWT** (JSON Web Tokens).

### **Dashboard**

- An overview of the user’s financial health:
  - Total income.
  - Total expenses.
  - Budget progress (e.g., % of budget used).

### **Income and Expense Tracking**

- Add, edit, and delete income and expense entries.
- Categorize transactions (e.g., "Rent," "Groceries").
- Include fields like amount, date, and notes for each transaction.

### **Budget Management**

- Set a monthly or category-based budget.
- Visualize spending vs. budget using **charts and graphs**.

### **Data Visualization**

- Interactive graphs for:
  - Spending trends over time.
  - Category breakdown (e.g., pie chart).
  - Budget progress.

### **Notifications**

- Alerts for overspending or reaching a certain budget threshold.

### **Responsive UI**

- Fully functional on both desktop and mobile devices.

---

## **Wireframe and Descriptions**

### **Login Page**

The login page allows users to securely access their accounts using a username and password.

![Login Page](wireframe/Financial%20Wireframe-1.png)

### **Dashboard**

The dashboard provides an overview of the user’s financial health, including:

- Total balance.
- Recent transactions.
- Spending categories.

![Dashboard](wireframe/Financial%20Wireframe-2.png)

### **Transactions Page**

This page allows users to:

- Add, edit, or delete transactions.
- View detailed transaction history with categories, amounts, and comments.

![Transactions Page](wireframe/Financial%20Wireframe-3.png)

### **Budgeting Page**

The budgeting page helps users:

- Set category-specific budgets.
- Track progress for each category (e.g., percentage of budget used).
- Create new budgets for specific categories

![Budgeting Page](wireframe/Financial%20Wireframe-4.png)

![Budgeting Choose Category](wireframe/Financial%20Wireframe-5.png)

![Budgeting Set Limit](wireframe/Financial%20Wireframe-6.png)

### **Reports Page**

(No Wireframe) The reports page provides visual insights into:

- Monthly spending trends.
- Budget performance.
- Category breakdowns.

---

## **Next Steps**

1. Set up the Flask backend:
   - Create the project structure.
   - Configure the PostgreSQL database connection.
   - Build user authentication endpoints using JWT.
2. Finalize frontend pages and start integrating them with backend APIs.
