🧪 Login Functionality Test Cases

## 📋 Overview
This document contains detailed **test cases** for verifying the login functionality of the website:  
🔗 [https://practicetestautomation.com/practice-test-login/](https://practicetestautomation.com/practice-test-login/)

The purpose of these test cases is to validate:
- Correct user authentication
- Error handling for invalid input
- UI behavior
- Field validation
- Security and usability aspects

---

## ✅ Test Environment
- **Test URL:** https://practicetestautomation.com/practice-test-login/  
- **Browser:** Chrome / Firefox / Edge  
- **OS:** Windows 10 / 11  
- **Test Type:** Manual  
- **Tester:** Gopal Hande  
- **Date:** November 2025

  # 🧩 Manual Test Cases

| **TC ID** | **Test Scenario** | **Pre-Requisites** | **Test Data** | **Test Steps** | **Expected Result** | **Actual Result** | **Status** |
|------------|------------------|--------------------|----------------|----------------|---------------------|------------------|-------------|
| **TC_01** | Verify user should be able to login with correct credentials | Web page loaded | Username: `student`<br>Password: `Password123` | 1. Navigate to https://practicetestautomation.com/practice-test-login/<br>2. Enter Username: `student`<br>3. Enter Password: `Password123` | Login should work with correct credentials; user should be logged in successfully | User logged in successfully | Pass |
| **TC_02** | Verify user login with incorrect username and correct password | Web page loaded | Username: `Student`<br>Password: `Password123` | 1. Navigate to login page<br>2. Enter Username: `Student`<br>3. Enter Password: `Password123` | User denied login; show message “Please enter valid username” | User denied login | Pass |
| **TC_03** | Verify user login with correct username and incorrect password | Web page loaded | Username: `student`<br>Password: `Student123` | 1. Navigate to login page<br>2. Enter Username: `student`<br>3. Enter Password: `Student123` | User denied login; show message “Please enter valid password” | User denied login | Pass |
| **TC_04** | Verify user login with incorrect username and incorrect password | Web page loaded | Username: `Student`<br>Password: `Student123` | 1. Navigate to login page<br>2. Enter Username: `Student`<br>3. Enter Password: `Student123` | User denied login; show message “Please enter valid username and password” | User denied login | Pass |
| **TC_05** | Verify user login with correct username and empty password | Web page loaded | Username: `student`<br>Password: *(blank)* | 1. Navigate to login page<br>2. Enter Username: `student`<br>3. Leave Password blank | User denied login; show message “Please enter password” | User denied login | Pass |
| **TC_06** | Verify user login with empty username and valid password | Web page loaded | Username: *(blank)*<br>Password: `Password123` | 1. Navigate to login page<br>2. Leave Username blank<br>3. Enter Password: `Password123` | User denied login; show message “Please enter username” | User denied login | Pass |
| **TC_07** | Verify login with both username and password fields empty | Web page loaded | Username: *(blank)*<br>Password: *(blank)* | 1. Navigate to login page<br>2. Leave both fields blank<br>3. Click Login | User denied login; show message “Please enter username and password” | User denied login | Pass |
| **TC_08** | Verify case sensitivity for username | Web page loaded | Username: `STUDENT`<br>Password: `Password123` | 1. Navigate to login page<br>2. Enter Username: `STUDENT`<br>3. Enter Password: `Password123` | User denied login; show message “Username is case-sensitive” | User denied login | Pass |
| **TC_09** | Verify login button is disabled when mandatory fields are empty | Web page loaded | Username: *(blank)*<br>Password: *(blank)* | 1. Navigate to login page<br>2. Leave all fields blank<br>3. Observe login button state | Login button should remain disabled/invisible | Login button inactive | Pass |

