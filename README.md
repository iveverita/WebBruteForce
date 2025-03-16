# WebBruteForce

# SimpleBruteForce Project

A lightweight educational framework for demonstrating web authentication vulnerabilities and security testing methodologies. This project is designed for educational purposes only to understand authentication workflows and security concepts.

## 🚨 Important Notice

This project is intended **ONLY** for:
- Educational purposes in controlled environments
- Testing systems you personally own
- Systems you have explicit written permission to test

Unauthorized testing of systems is illegal and unethical. Always practice responsible security testing.

## 📋 Project Overview

This project consists of three main components:

1. **Web Interface (index.html)**: A simple login and registration system built with HTML, CSS, and JavaScript
2. **Backend Server (server.py)**: A Flask server that handles authentication requests
3. **Testing Script (brute_force.py)**: A demonstrative tool that shows how automated login attempts work

## 🛠️ Setup Instructions

### Prerequisites
- Python 3.6 or higher
- pip (Python package manager)

### Step 1: Clone the Repository
```bash
git clone https://github.com/yourusername/SimpleBruteForce.git
cd SimpleBruteForce
```

### Step 2: Install Dependencies
```bash
pip install flask requests
```

### Step 3: Prepare a Wordlist (Optional)
For educational testing, you can use a small custom wordlist:
```bash
echo "password123" > wordlist.txt
echo "admin" >> wordlist.txt
echo "12345" >> wordlist.txt
```

For more comprehensive testing, you can download common wordlists like "rockyou.txt" which are available in security testing distributions like Kali Linux.

## 🚀 Running the Project

### Step 1: Start the Web Server
```bash
python server.py
```
This will start the Flask server at http://127.0.0.1:8000

### Step 2: Access the Web Interface
Open your browser and navigate to http://127.0.0.1:8000

### Step 3: Register a Test User
Create a test account through the registration form on the web interface.

### Step 4: Run the Testing Script (Educational Purposes Only)
```bash
python brute_force.py
```
Follow the prompts to enter the username, wordlist path, and login URL.

## 💡 How It Works

### Authentication System
- Users can register accounts with usernames and passwords
- Registered users are stored in a JSON file (users.json)
- Login attempts are validated against stored credentials

### Security Testing Script
- Reads passwords from a wordlist file
- Attempts to login using the provided username and each password
- Reports success or failure after attempting all passwords
- Monitors time elapsed and number of attempts

## 🔒 Security Considerations

In a real-world application, you would want to implement:
- Password hashing (using bcrypt or similar)
- Account lockout after multiple failed attempts
- CAPTCHA protection against automated attempts
- Rate limiting of login requests
- HTTPS for secure communication
- Two-factor authentication

## 📚 Learning Resources

To learn more about web security:
- [OWASP Authentication Best Practices](https://owasp.org/www-project-top-ten/)
- [Web Security Academy](https://portswigger.net/web-security)
- [Mozilla Web Security Guidelines](https://infosec.mozilla.org/guidelines/web_security)

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 📧 Contact

If you have any questions about this educational project, please contact me at your.email@example.com or through my GitHub profile.
