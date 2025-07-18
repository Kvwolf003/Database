# Database


A simple PHP-MySQL web application that allows users to be added to a database and toggle their status (ON/OFF) using a web interface.

## 📦 Features

- Add users with name and age
- Display all users in a table
- Toggle user status between ON and OFF
- Built with PHP, MySQL, HTML, and CSS
- Uses XAMPP (Apache + MySQL stack)

---

## 🚀 Installation

### 1. Requirements
- Linux Mint (or any OS with XAMPP)
- XAMPP installed and running

### 2. Set Up XAMPP
- Start *Apache* and *MySQL* from the XAMPP Control Panel
- Open phpMyAdmin: http://localhost/phpmyadmin

### 3. Create the Database

1. Create a new database called status_db
2. Run this SQL in the SQL tab:

```sql
CREATE TABLE users (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(50),
  age INT,
  status TINYINT DEFAULT 0
);


⸻

🧩 Project Structure

/opt/lampp/htdocs/user_status/
│
├── index.php      # Main application file (form + table + toggle logic)
├── db.php         # Database connection file
├── style.css      # Optional: your custom CSS file


⸻

✏️ How to Use
	1.	Visit the app in your browser:

http://localhost/user_status

	2.	Use the form to add a new user (name + age)
	3.	View all users in a table
	4.	Click the “Toggle” button to switch the user’s status between ON and OFF

⸻

🛠 Technologies Used
	•	PHP
	•	MySQL (via phpMyAdmin)
	•	HTML / CSS
	•	XAMPP (Apache & MySQL server)

⸻

📁 Notes
	•	The database connection is configured in db.php:

$conn = new mysqli("localhost", "root", "", "status_db");

	•	Make sure MySQL is running before using the app.

⸻

📸 Screenshots (Optional)

Add screenshots of your form and table here for demo purposes.

⸻

🤝 License

This project is open source and free to use for learning and experimentation.
