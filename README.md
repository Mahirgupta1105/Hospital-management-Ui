🏥 Hospital Management System (Java + Swing + MySQL)
A GUI-based Hospital Management System developed in Java (Swing) with MySQL database connectivity using JDBC. This project allows users to manage doctors, patients, and appointments from a user-friendly interface.

✨ Features
🔐 Secure Login System (admin panel)
👨‍⚕️ Add Doctor with specialization and contact
🧑‍🤝‍🧑 Register Patients with age, gender, and contact
📅 Book Appointments between patients and doctors
📋 View all records using tabbed tables (Doctors, Patients, Appointments)
🛠 Technologies Used
Java (JDK 8 or higher)
Swing for GUI
JDBC for MySQL connectivity
MySQL (Workbench or CLI)
🗂️ Project Structure

⚙️ How to Run
1. ✅ Requirements
Java (JDK 8 or higher)
MySQL Server
MySQL Workbench (or CLI)
VS Code / IntelliJ / Eclipse
2. 🧬 Setup Database
Open MySQL Workbench
Create a new schema: hospital_db
Import hospital.sql file provided in this repo
CREATE TABLE users ( id INT AUTO_INCREMENT PRIMARY KEY, username VARCHAR(50), password VARCHAR(50) );

CREATE TABLE doctors ( id INT AUTO_INCREMENT PRIMARY KEY, name VARCHAR(100), specialization VARCHAR(100), contact VARCHAR(100) );

CREATE TABLE patients ( id INT AUTO_INCREMENT PRIMARY KEY, name VARCHAR(100), age INT, gender VARCHAR(10), contact VARCHAR(100) );

CREATE TABLE appointments ( id INT AUTO_INCREMENT PRIMARY KEY, patient_id INT, doctor_id INT, date DATE );

-- Sample admin user INSERT INTO users(username, password) VALUES ('admin', 'admin');
