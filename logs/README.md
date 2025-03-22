# SIT737 - 4.1P: Calculator Microservice

This project is part of SIT737 - Cloud Native Application Development (Practical 4.1P). The goal is to build a simple calculator microservice using Node.js and Express that performs basic arithmetic operations: addition, subtraction, multiplication, and division. It also includes error handling and logging with Winston.

---

## Step-by-Step Instructions

### 1. Install Prerequisites

Ensure you have the following installed on your system:

- Node.js: https://nodejs.org/en/download/
- Git: https://git-scm.com/
- Visual Studio Code: https://code.visualstudio.com/

---

### 2. Clone the Repository

```bash
git clone https://github.com/mariyatheresa/sit737-2025-prac4p.git
cd sit737-2025-prac4p

### 2. Initialize and Install Dependencies
npm init -y
npm install express winston
npm install

### 3. Run the Application
node app.js

we can see :"Calculator microservice running on http://localhost:2002"


### REST API Endpoints
Each endpoint accepts two query parameters: val1 and val2.


GET	/add	"Adds two numbers"	/add?val1=10&val2=5
GET	/subtract	"Subtracts two numbers"	/subtract?val1=10&val2=5
GET	/multiply	"Multiplies two numbers"	/multiply?val1=10&val2=5
GET	/divide	"Divides two numbers"	/divide?val1=10&val2=5

### Logging with Winston
The service uses Winston to log:
IP address
Request method
Operation details

Errors (e.g., invalid input, division by zero)

Log files:
logs/error.log – Contains all error-level logs

logs/combined.log – Contains all logs (info, errors, etc.)


