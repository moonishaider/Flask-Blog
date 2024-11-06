# Flask Blog Application with DevOps Integration

## Project Overview
This project is a microblogging web application built with Flask, featuring user authentication, blog posts, followers, and pagination. It serves as an excellent platform to integrate DevOps practices like CI/CD, containerization, and infrastructure automation.

---

## Features
- **User Authentication:** Secure user registration and login system.
- **Blog Posts:** Create, edit, and delete blog posts.
- **Followers System:** Users can follow and unfollow each other.
- **Pagination:** Efficient handling of large datasets.

---

## Prerequisites
- Python 3.x installed on your system.
- A virtual environment for managing dependencies.
- Docker installed for containerization.
- Optional: GitHub Actions for CI/CD, Terraform for IaC.

---

## Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/miguelgrinberg/microblog.git
cd microblog
```
### 2. Set Up a Virtual Environment
```bash
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```
### 3. Install Dependencies
```bash
pip install -r requirements.txt
```
### 4. Configure Environment Variables
```bash
FLASK_APP=microblog.py
FLASK_ENV=development
SECRET_KEY=your_secret_key
DATABASE_URL=sqlite:///app.db
```
### 5. Initialize the Database
```bash
flask db upgrade
```
### 6. Run the Application
```bash
flask run
```
