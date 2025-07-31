# 📸 SnapAttend – A Next-Gen Attendance Monitoring Solution

SnapAttend is an AI-powered smart attendance system designed to automate and streamline the attendance tracking process for educational institutions. By using facial recognition technology and real-time image processing, SnapAttend minimizes manual errors and maximizes efficiency.

---

## 🔑 Login Credentials

To access the app for testing/demo purposes, use the following credentials:

- **Email**: `ssm@gmail.com`
- **Password**: `dkte123`

---

## 🚀 Key Features

- 📷 **Facial Recognition-Based Attendance** – Just capture a snapshot; the app identifies students and marks attendance.
- 📊 **Real-Time Analytics** – Visualize attendance trends for students and classes.
- 📤 **Excel Report Generation** – Export attendance data in Excel format.
- 📲 **Notifications** – Automatically notify parents of absentees.
- 📚 **Class Selection** – Faculty can choose specific classes before capturing attendance.
- 📩 **Attendance Reminders** – Admins can request faculty to submit pending attendance.
- 🔐 **Login System** – Role-based access for Admin, Faculty, and Parents.

---

## 🖼️ Screenshots

<!-- > Make sure to upload these images in a folder like `assets/screenshots/`. -->

### 🔐 Login Page
![Login](assets/screenshots/login_page.png)

### 🎯 Dashboard
![Dashboard](assets/screenshots/dashboard.png)

### 📈 Analytics Report
![Analytics](assets/screenshots/analytics.png)

---

## 🧠 Architecture Overview

- **Frontend (Flutter)**:
  - Platform-independent UI for Android, iOS, Web, etc.
  - Clean navigation between login, dashboard, attendance pages.
  
- **Backend (Python + Flask)**:
  - REST API to handle authentication, image processing, data storage, and retrieval.
  
- **Database (MongoDB)**:
  - Stores user data, attendance logs, reports, etc.

---

## 🛠️ Tech Stack

| Layer       | Technology Used                |
|------------|---------------------------------|
| Frontend   | Flutter                         |
| Backend    | Python, Flask, face_recognition |
| Database   | MongoDB Atlas                   |
| Deployment | Docker, Docker Compose          |
| Hosting    | GitHub                          |

---

## 📦 Installation & Setup

### 📁 Clone Both Repositories

```bash
git clone https://github.com/SnapAttend/Backend.git
git clone https://github.com/SnapAttend/Frontend.git
```
### 🐳 Backend (Flask API with Docker)

Ensure you are in the backend directory before running the Docker commands.

```bash
cd Backend
docker-compose up --build
```
This will spin up the Flask app and connect to MongoDB automatically.
### 📱 Frontend (Flutter App)
Navigate to the Flutter app folder:
```bash
cd Frontend
flutter pub get
flutter run
```
To build APK:
```bash
flutter build apk --release
```
## 📂 Project Structure
### 🔁 Backend

```pgsql
Backend/
├── server.py
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
```
### 📱 Frontend
```bash
Frontend/
├── lib/
├── android/
├── ios/
├── pubspec.yaml
├── README.md
├── .env
```
---
## 📥 APK Download

You can attach this in GitHub under the [**Releases**](https://github.com/SnapAttend/Frontend/releases) tab or create a direct link:

🔗 [**Download SnapAttend APK**](https://github.com/SnapAttend/Frontend/releases/download/v1.0.0/snapattend.apk)
---
## 🧪 Testing

- Login using the demo credentials.
- Select a class and capture a sample image.
- Verify recognized faces and generated report.
- Check analytics and attendance logs.
---
<!-- ## 📝 License
This project is licensed under the MIT License. See the LICENSE file for details.
--- -->
## 📬 Contact

For any queries, feedback, or collaboration opportunities related to **SnapAttend**, feel free to reach out:

📧 **Email**: megaaproject2024@gmail.com  
🐙 **GitHub**: [SnapAttend](https://github.com/SnapAttend)  
📄 **Issues**: [Report an Issue](https://github.com/SnapAttend/Frontend/issues)

Alternatively, contact any of the core contributors directly:

- [Prajakta Darekar](https://github.com/prajudarekar04)
- [Pooja Hanamane](https://github.com/poojah08)
- [Pratik Kumbhar](https://github.com/pk049)
- [Piyusha Shinde](https://github.com/piyushashinde01)
- [Akanksha Yedrave](https://github.com/akankshayedrave)
---
