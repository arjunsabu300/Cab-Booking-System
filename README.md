# 🚖 Cab Booking System

## 📌 Overview
The **Cab Booking System** is a web-based platform that allows users to book cabs conveniently. The system provides features like user registration, cab booking, fare calculation, driver availability, and a map-based pickup/dropoff selection. The backend is powered by **Flask** and **MySQL**, with **Open Route Service (ORS)** integrated for map functionality.

## ✨ Features
✅ **User Authentication**: Register and log in securely.  
✅ **Cab Booking**: Enter pickup and drop locations, select date and time, and book a cab.  
✅ **Fare Calculation**: Base fare of **₹10 per km**.  
✅ **Driver Management**: View available drivers from the database.  
✅ **Map Integration**: Select locations and find routes using **ORS**.  
✅ **Booking History**: View past rides and details.  

## 🛠 Technologies Used
🚀 **Backend**: Flask (Python)  
🎨 **Frontend**: HTML, CSS, JavaScript  
🗄 **Database**: MySQL  
🗺 **Map Service**: Open Route Service (ORS)  
☁ **Hosting**: Clever Cloud  

## 📊 Database Schema
### 📌 `users` Table
| 🆔 Column   | 🗂 Type         | 📝 Description |
|------------|---------------|----------------|
| 🆔 userid  | INT (PK)      | Unique user ID |
| 👤 username | VARCHAR(100)  | User's name |
| 🔑 password | VARCHAR(255)  | Hashed password |

### 📌 `booking` Table
| 🆔 Column         | 🗂 Type                | 📝 Description |
|------------------|-------------------|-------------|
| 🆔 bookingID     | INT (PK) AUTO_INCREMENT | Unique booking ID |
| 📍 pickup_location | VARCHAR(150)       | Pickup point |
| ⏰ pickup_time   | TIME               | Scheduled pickup time |
| 📅 pickup_date   | DATE               | Scheduled pickup date |
| 🏁 drop_location  | VARCHAR(150)       | Drop-off location |
| 👥 no_of_people  | INT                | Number of passengers |
| 💰 amount        | DECIMAL(10,5)      | Calculated fare |

## 🚀 Installation & Setup
1. **Clone the repository** 📥:
   ```bash
   git clone https://github.com/your-repo/cab-booking.git
   cd cab-booking
   ```
2. **Create a virtual environment** 🌐:
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. **Install dependencies** 📦:
   ```bash
   pip install -r requirements.txt
   ```
4. **Set up the database** 🗄:
   - Create a **MySQL database** and import `schema.sql`.
   - Update `config.py` with database credentials.
5. **Run the application** ▶:
   ```bash
   python app.py
   ```
6. **Access the system** 🌍:
   Open https://cab-booking-system-7c5e.onrender.com/login in a browser.

## 🔮 Future Enhancements
🚖 Integration with payment gateways.  
📍 Real-time driver tracking.  
🤖 AI-based fare optimization.  

## 👨‍💻 Contributors
- **Arjun Sabu** - Developer & Maintainer  

## 📜 License
This project is licensed under the **MIT License**.

