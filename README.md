# Lint-Coffe-Shop
A Python GUI-based product management system with MSSQL integration, user authentication, email recovery, and camera support.
# Term Project – Python GUI Application with MSSQL Integration

This project is a desktop-based GUI application built with Python, providing product and user management capabilities through an MSSQL database. It incorporates user authentication, password recovery via email, product addition with image and date selection, and real-time camera access using OpenCV.

## 👨‍💻 Contributor
- Tolga Ünlü
Install dependencies:
pip install pyodbc
pip install smtplib
pip install ssl
pip install opencv-python
pip install numpy
pip install Pillow
pip install EmailMessage
pip install tkcalendar
## 🧰 Technologies & Libraries Used

- `tkinter` – GUI Design  
- `pyodbc` – MSSQL Connection  
- `smtplib` & `EmailMessage` – Email Sending  
- `opencv` – Camera Integration  
- `Pillow` – Image Handling  
- `tkcalendar` – Calendar Widget  
- `MSSQL` – Database Backend

## 🛠 Features

- **User Login with Combobox Selection**  
  - Users are listed via a `ttk.Combobox`, and authentication is handled through `tk.Entry`.

- **Password Recovery via Email**  
  - If a user forgets their password, it is sent to their registered email address using `SMTP`.

- **User Management**  
  - New users can be added through a GUI form. The system prevents empty fields from being submitted.

- **Product Management**  
  - Users can view product details including images.
  - A new product can be added with the help of a form that includes:
    - `DateEntry` calendar selector
    - PNG image upload using `filedialog`
    - Raw Material management via additional frames
    - Image preview before upload

- **Real-time Camera Access**  
  - OpenCV is used to access and display live camera feed from within the app.

## 🗂 MSSQL Configuration

To run the project locally:

1. Install **MSSQL** and load the provided `.bak` database backup.
2. Update the connection string:
```python
db.connect('Driver={SQL Server};'
           'Server=YOUR-PC-NAME;'
           'Database=TermProjectOOP;'
           'Trusted_Connection=yes;')
