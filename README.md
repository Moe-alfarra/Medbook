🏥 Hospital Booking System — MedBook

MedBook is a hospital booking system that allows patients from different hospitals to easily book appointments with specific doctors.

🌐 Live Demo: https://medbook1.onrender.com

⚙️ Project Overview

🧩 Frontend (Website)
Developed using HTML, CSS, and JavaScript.
Main Pages:
  index.html — Home page
  about.html — About the system
  booking.html — Appointment booking page
  confirm.html — Booking confirmation
  doctors.html — Doctor listings
  login.html — User authentication
  profile.html — Patient dashboard/profile

🧠 Backend (Server)
Backend built using Flask (Python) and hosted on Render.
Main files:
  table.py — Main Flask server
  .env — Environment variables (e.g., database credentials, secret keys)
  requirements.txt — Python dependencies
  venv/ — Virtual environment directory

🗄️ Database
Type: PostgreSQL
Host: Neon.tech
  (AWS-backed managed PostgreSQL)
Main Entities (Tables):
  Patients
  Doctors
  Hospitals
Relationships:
  appointments — connects patients to doctors
  doctors_availability — tracks doctor schedules

☁️ Hosting and Deployment
Frontend: Hosted on Render
Backend API: Flask app hosted on Render
Database: Neon PostgreSQL (AWS-hosted)

NOTE: All services are actively monitored to ensure public availability.

🖥️ Running the Project Locally
Follow these steps to set up and run the system on your local machine:
  1) Create a directory on your Desktop.
  2) Download or clone the repository into that directory.
  3) Navigate to the folder in your terminal.
  4) Create a virtual environment in cmd:
      python -m venv venv
  5) Activate the virtual environment:
      venv\Scripts\activate  # On Windows
      source venv/bin/activate  # On macOS/Linux
  6) Install dependencies:
      pip install -r requirements.txt
  7) Run the backend server locally using Waitress:
      waitress-serve --listen=0.0.0.0:5000 table:app
  8) Access the website:
      If hosted version: https://medbook1.onrender.com
      If local HTML files: open them in your browser, but update API calls to
      http://127.0.0.1:5000 or http://localhost:5000 in your JS files.
