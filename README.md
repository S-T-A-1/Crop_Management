🌾 Crop Management System

Crop Management System is a Python-based application with a Tkinter GUI that helps manage crop data. It supports manual record entry and bulk insertion of up to 100,000 random crop records using MySQL for backend storage.

🚀 Features
	•	Manual Data Entry: Add crop details like planting/harvest dates, growth stage, pest control measures, and yield prediction.
	•	Bulk Data Insertion: Generate and insert 100,000 random crop records for testing or analysis.
	•	Live Data View: Displays the latest 20 records in a scrollable table.

🛠️ Installation
	1.	Clone the repository:

git clone https://github.com/your-username/Crop-Management-System.git
cd Crop-Management-System


	2.	Install the required libraries:

pip install mysql-connector-python faker


	3.	Create the MySQL database and table:

CREATE DATABASE crop_management;

USE crop_management;

CREATE TABLE crops (
    id INT AUTO_INCREMENT PRIMARY KEY,
    crop_name VARCHAR(50),
    planting_date DATE,
    harvest_date DATE,
    growth_stage VARCHAR(50),
    pest_control_measures VARCHAR(100),
    yield_prediction INT
);


	4.	Update the database credentials in the script:

DB_CONFIG = {
    "host": "localhost",
    "user": "root",
    "password": "your_password",
    "database": "crop_management"
}


	5.	Run the application:

python crop_management.py



📘 Usage
	•	Insert Record: Fill in the crop details and click Insert Record.
	•	Bulk Insert: Click Insert 100,000 Random Records to generate and insert large datasets.
	•	View Records: The latest 20 records are displayed in a table.
