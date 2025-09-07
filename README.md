# Playwright Automation Task – Login & Registration Scenarios

## 📌 Overview
This project contains automated test cases for a sample web application using **Playwright** with **TypeScript**.  
It follows the **Page Object Model (POM)** design pattern for maintainability and scalability.  
Test results are reported using **Allure Report**, and test execution is recorded as videos.  

### ✅ Automated Test Cases
1. **Test Case 3:** Login User with incorrect email and password  
   - Verifies error handling when invalid credentials are entered.  

2. **Test Case 4:** Logout User  
   - Ensures a logged-in user can successfully log out.  

3. **Test Case 5:** Register User with existing email  
   - Checks validation when trying to register with an already registered email.  

---

## 🗂 Project Structure
```
AutomationTask-Playwright/
│── PageModel/              # Page Object Models
│── TestCases/Specs/        # Test cases
│── playwright.config.ts    # Playwright configuration
│── package.json            # Dependencies and scripts
│── README.md               # Project documentation
│── allure-report/          # Generated Allure report (HTML)
│── videos/                 # Test execution recordings
```

---

## ⚙️ Setup Instructions

### 1. Prerequisites
- [Node.js](https://nodejs.org/) (LTS recommended)
- npm (comes with Node.js)
- [Allure Commandline](https://docs.qameta.io/allure/) (to generate reports)  
  Install via npm:
  ```bash
  npm install -g allure-commandline --save-dev
  ```

### 2. Install Dependencies
From the project root, run:
```bash
npm install
```

---

## ▶️ Running the Tests
Run all tests:
```bash
npx playwright test
```

Run a specific test case (example: Test Case 3):
```bash
npx playwright test TestCases/Specs/loginTCs.spec.ts -g "Login User with incorrect email and password"
```

---

## 📊 Generating a New Allure Report

1. After running tests, raw results will be saved in `./allure-results`.  
2. Generate the HTML report:
   ```bash
   allure generate ./allure-results --clean -o ./allure-report
   ```
3. Open the report in your browser:
   ```bash
   allure open ./allure-report
   ```

---

## 🎥 Test Evidence
- **Videos:** All test executions are recorded and available in the `videos/` folder.  
- **Allure Report:** Detailed results (including steps, and failures) available in `allure-report/` or attached as `index.html`.  

---

## 🤝 Notes
- Tests are written using the **Page Object Model (POM)** for better reusability and clarity.  
- Allure report provides detailed visibility into:
  - Passed/Failed test cases
  - Execution steps

---

## 📌 Author
Ahmed Mahmoud Eissa  
