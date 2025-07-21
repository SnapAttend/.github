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

> Make sure to upload these images in a folder like `assets/screenshots/`.

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
git clone https://github.com/SnapAttend/Android_App/backend.git
git clone https://github.com/SnapAttend/Android_App/frontend.git
```
### 🐳 Backend (Flask API with Docker)

Ensure you are in the backend directory before running the Docker commands.

```bash
cd backend
docker-compose up --build
```
This will spin up the Flask app and connect to MongoDB automatically.
### 📱 Frontend (Flutter App)
Navigate to the Flutter app folder:
```bash
cd frontend
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
backend/
├── server.py
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
```
### 📱 Frontend
```bash
frontend/
├── lib/
├── android/
├── ios/
├── pubspec.yaml
├── README.md
├── .env
```
---
## 📥 APK Download

You can attach this in GitHub under the [**Releases**](https://github.com/SnapAttend/Android_App/frontend/releases) tab or create a direct link:

🔗 [**Download SnapAttend APK**](https://github.com/SnapAttend/Android_App/frontend/releases/download/v1.0.0/snapattend.apk)
---
## 🧪 Testing

- Login using the demo credentials.
- Select a class and capture a sample image.
- Verify recognized faces and generated report.
- Check analytics and attendance logs.
---
## 📝 License
This project is licensed under the MIT License. See the LICENSE file for details.
---
## 📬 Contact

For any queries, feedback, or collaboration opportunities related to **SnapAttend**, feel free to reach out:

📧 **Email**: megaaproject2024@gmail.com  
🐙 **GitHub**: [SnapAttend](https://github.com/SnapAttend/Android_App)  
📄 **Issues**: [Report an Issue](https://github.com/SnapAttend/Android_App/frontend/issues)

Alternatively, contact any of the core contributors directly:

- [Prajakta Darekar](https://github.com/prajudarekar04)
- [Pooja Hanamane](https://github.com/poojah08)
- [Pratik Kumbhar](https://github.com/pk049)
- [Piyusha Shinde](https://github.com/piyushashinde01)
- [Akanksha Yedrave](https://github.com/akankshayedrave)
---
<!--
# SnapAttend - A Next-Gen Attendance Monitoring Solution

SnapAttend is a smart attendance system designed to automate and streamline attendance management using facial recognition technology. Developed for educational institutions, it allows faculty to capture classroom images, automatically identify students, and mark attendance with minimal effort.

The system enhances efficiency and transparency by generating attendance reports, notifying parents of absentees, and offering analytical insights — all through a mobile-friendly platform built with Flutter and powered by a robust Python backend.
---
## Key Features

- Facial recognition-based attendance marking from classroom snapshots.
- Real-time analytics and insights into attendance patterns.
- Excel/PDF report generation for administrative review.
- Notifications to parents for absent students.
- Faculty-specific attendance submission requests and tracking.
- Prior defaulter list generation and manual override support.
- Secure login system for faculty users.

### Demo Login Credentials

To explore the app's features, you can use the following demo login credentials:

- **Email:** ssm@gmail.com  
- **Password:** dkte123
---
## Problem Definition

Traditional attendance systems are time-consuming, error-prone, and prone to manipulation. Manual roll calls waste valuable lecture time, and hardware-based biometric systems can be expensive, unhygienic, and dependent on physical contact.

Educational institutions need a contactless, efficient, and reliable solution for managing attendance records in real-time.

**SnapAttend** addresses this problem by leveraging facial recognition and computer vision. With just a snapshot, the system detects and identifies students, marks attendance, and synchronizes records instantly — eliminating manual errors and boosting productivity.

## Aim

To develop a smart and automated attendance system using facial recognition technology that reduces the time and effort required for manual attendance.

## Objectives

- Automate student attendance using computer vision.
- Provide real-time insights and attendance analytics.
- Generate downloadable attendance reports.
- Notify parents of absentee students.
- Offer a user-friendly, mobile-first experience for faculty.
---
## Scope and Limitations

### Scope

- Mobile application built using Flutter for Android and iOS platforms.
- Backend built with Python and Flask, integrated with facial recognition and image processing tools.
- Real-time facial recognition using OpenCV and face_recognition libraries.
- Role-based access for faculty and admin users.
- Notification system to inform parents about student absences.
- Data analytics and reports for attendance trends.

### Limitations

- Good lighting conditions are required for accurate facial recognition.
- High-quality camera needed to capture clear student images.
- Internet connectivity is essential for real-time data synchronization.
- System performance may be affected by crowded or obstructed classrooms.
---
## Screenshots

### 🔐 Login Page
![Login Page](assets/screenshots/login_page.png)

### 🧑‍🏫 Faculty Dashboard
![Faculty Dashboard](assets/screenshots/dashboard.png)

### 📊 Attendance Report
![Attendance Report](assets/screenshots/attendance_report.png)

---
## System Architecture

SnapAttend is designed using a modular, cross-platform architecture with clear separation between frontend, backend, and database layers.

### Backend (Python + Flask + MongoDB)

- RESTful API built using Flask.
- Handles authentication, face recognition, and attendance logic.
- Uses `face_recognition` and OpenCV libraries for facial encoding and matching.
- MongoDB Atlas used for cloud-based, NoSQL data storage.
- Dockerized for easy deployment and environment consistency.

**Main API functionalities:**
- User login and authentication.
- Face encoding and recognition.
- Attendance marking and retrieval.
- Lecture/session logs.
- Subject/class data management.

**Repository:** [SnapAttend Backend](https://github.com/YourOrg/snapattend-backend)

### Frontend (Flutter)

- Cross-platform mobile app supporting Android and iOS.
- Role-based dashboard for faculty and admin.
- Features include camera integration, class selection, attendance capture, analytics, and profile management.
- Communicates with backend through secure REST API calls.

**Main Screens:**
- Login Page
- Dashboard
- Class Selection
- Attendance Capture
- Analytics & Reports
- Profile

**Repository:** [SnapAttend Frontend](https://github.com/YourOrg/snapattend-frontend)
---
## Technologies Used

| Layer       | Technologies Used                            |
|-------------|----------------------------------------------|
| Frontend    | Flutter, Dart                                |
| Backend     | Python, Flask, OpenCV, face_recognition      |
| Database    | MongoDB Atlas (NoSQL, cloud-hosted)          |
| DevOps      | Docker, GitHub Actions (CI/CD)      |
| Tools/Libraries | Dlib, NumPy, face_recognition, Firebase Auth (for login) |
---
## Implementation Details

SnapAttend is implemented using a modular, scalable, and cross-platform approach. Below is a breakdown of each major component.

### Frontend – Flutter (Cross-Platform)

**Language:** Dart  
**Platform Support:** Android, iOS (Web optional)

**Key Pages:**
- **LoginPage** – User authentication using Firebase Auth.
- **Dashboard** – Main interface for faculty/admin users.
- **ClassSelectionPage** – Dropdown to select subject/class.
- **AttendanceCapturePage** – Captures classroom photo via camera.
- **AnalyticsPage** – Displays attendance trends and insights.
- **RecordsPage** – View/download attendance history.
- **ProfilePage** – View/edit user information.

**Core Features:**
- Material Design UI
- Secure login/logout flow
- Camera integration for face capture
- REST API integration with backend
- Excel/PDF export functionality

---

### Backend – Python (Flask + Face Recognition)

**Framework:** Flask  
**Core Libraries:** face_recognition, OpenCV, NumPy, Flask-CORS

**Key Modules:**
- `face_detection.py` – Detects faces from input image.
- `face_recognition.py` – Matches faces with known encodings.
- `attendance_manager.py` – Marks attendance and logs metadata.
- `notification_service.py` – Sends SMS/email notifications (optional).

**API Endpoints Examples:**
- `POST /login` – User authentication.
- `POST /recognize_faces` – Accepts image, returns identified students.
- `POST /mark_attendance` – Saves attendance in database.
- `GET /attendance_summary` – Fetches attendance records.

---

### Database – MongoDB Atlas

**Type:** NoSQL (Document-Oriented)  
**Hosted:** Cloud-based via MongoDB Atlas

**Main Collections:**
- `Users` – Faculty and student user profiles.
- `Encodings` – Stored facial encodings per student.
- `AttendanceRecords` – Marked attendance logs per class.
- `SessionLogs` – Data about each lecture/session event.
- `Subjects` – Class-subject mappings and metadata.
---
## Applications

SnapAttend can be deployed in various educational and organizational environments:

- **Colleges & Universities**: Automates student attendance and analytics across multiple departments.
- **Schools**: Keeps parents informed about attendance while reducing manual work for teachers.
- **Training Institutes**: Tracks participant engagement with minimal setup.
- **Corporate Training Sessions**: Ensures attendance monitoring during employee onboarding or workshops.
- **Hybrid Learning Environments**: Useful in classrooms where physical and remote students are both present.
---
## Installation Guide

To run the SnapAttend project locally, follow these steps:

### 1. Clone Repositories

Clone both the backend and frontend repositories:

Backend:
    git clone https://github.com/<org-name>/snapattend-backend.git

Frontend:
    git clone https://github.com/<org-name>/snapattend-frontend.git

### 2. Backend Setup (Flask + Docker)

1. Navigate to the backend folder:
       cd snapattend-backend

2. (Optional) Create virtual environment:
       python -m venv venv
       venv\Scripts\activate  (for Windows)

3. Install required packages:
       pip install -r requirements.txt

4. Or run using Docker:
       docker-compose up --build

5. Access server:
       Flask app runs on http://localhost:5000 by default.

### 3. Frontend Setup (Flutter)

1. Navigate to frontend directory:
       cd snapattend-frontend

2. Get Flutter packages:
       flutter pub get

3. Run the app:
       flutter run

   > You can also open the `.apk` file directly to install on an Android device.

### 4. APK File (Optional)

You can find the latest APK build in the `releases/` folder of the frontend repo or [provide a direct GitHub release link if hosted].

### 5. Login Credentials (For Demo)

Use the following credentials to log in as a test user:

    Email:    ssm@gmail.com
    Password: dkte123
---
## Contact / Maintainers

SnapAttend is developed and maintained by the following team members:

- [Prajakta Darekar](https://github.com/prajudarekar04)
- [Pooja Hanamane](https://github.com/poojah08)
- [Pratik Kumbhar](https://github.com/pk049)
- [Piyusha Shinde](https://github.com/piyushashinde01)
- [Akanksha Yedrave](https://github.com/akankshayedrave)

For any queries or collaboration opportunities, feel free to reach out via GitHub.
---
-->
