# Financial Management Application Documentation

## **Overview**
This document outlines the features, functionalities, and implementation details of a financial management application designed to help users track their income, expenses, and transactions. The application includes categories for transactions, subscription-based features, and built-in security measures to protect user data.

---

## **Features**

### **User Registration and Authentication**
1. **Registration Process**:
   - Users register using:
     - **Email**
     - **Strong Password** (encrypted with salt on the backend)
     - **Referral Code** (optional)
   - Once registered, an **OTP** is sent to the user's email for verification.
   - Only after OTP verification will the user’s account be activated and accessible.

2. **Login**:
   - Users can log in after successful registration and OTP verification.

3. **Security**:
   - Passwords are stored securely using **encryption with salt**.
   - Users are required to set up a **PIN** for added security.
   - **Dark Mode** is available for better user experience.

4. **Permissions**:
   - **Notification Permission**: Used for sending transaction-related notifications.
   - **SMS Permission**: Added for future use (not active currently).

---

### **Subscription-Based Model**
1. **Subscription Tiers**:
   - **Basic Subscription**
   - **Premium Subscription**

2. **Current Access**:
   - All menus are visible without subscription for now.
   - Future updates will require monthly subscriptions to access premium features.

3. **Ads**:
   - The application supports advertisements.

---

### **Core Functionalities**

#### **Home Screen**:
- Displays an overview of financial data, including:
  - **Income and Expense Details**:
    - Total Income
    - Total Expenses
    - Maximum Income
    - Maximum Expense
  - **Charts**:
    - Visual representation of income and expenses.
  - **Top 5 Categories**:
    - Categories with the highest spending.
  - **Last 5 Transactions**:
    - Details include category, amount, type (income/expense), and timestamp.

---

#### **Add Transaction**:
- **Fields for Adding a Transaction**:
  - Amount
  - Category (select from existing or create a new one)
  - Paid To / Received From
  - Transaction Mode (e.g., cash, card, UPI, etc.)
  - Transaction Type (Income or Expense)
  - Transaction Date and Time
  - Created Datetime (automatically set)

- Transactions are:
  - Editable: Users can modify any transaction via the **Transaction History** screen.
  - Deletable: Users can delete transactions by swiping left in the **Transaction History** screen.

---

#### **Transaction History**:
- Displays a list of all user transactions with:
  - Filters for searching transactions by:
    - Date
    - Category
    - Transaction Mode
  - **Delete Functionality**:
    - Swipe left to reveal the delete button.
  - **Edit Functionality**:
    - Tap to open the edit screen for modifying transactions.
- Top section displays:
  - Total Income
  - Total Expenses

---

#### **Calendar Screen**:
- Displays transactions date-wise using a calendar view.
- On clicking a specific date, all transactions for that day are listed.

---

#### **Manage Categories**:
- **Features**:
  - Add new categories (fields: Name, Description).
  - Update existing categories.
  - Delete custom categories.
  - **Built-In Categories**: Provided by the app, these cannot be deleted or edited.

---

#### **Expenses Category**:
- View spending details categorized by category.
- Check detailed expenses for a specific category.

---

#### **Profile Screen**:
- Displays user details:
  - Name
  - Phone Number
  - State and Country
  - Monthly Income
  - Subscription Plan
  - Date of Birth
- Manage options:
  - Update Password
  - Edit Profile Information

---

#### **Analytical Screen**:
- **Coming Soon**: Will allow users to analyze their transactions.

---

#### **Savings Screen**:
- **Coming Soon**: Users will manage savings and financial goals.

---

#### **FAQ Screen**:
- Information on:
  - Data collection and usage for managing transactions.
  - Security and privacy practices.

---

### **Additional Features**
1. **Dark Mode**: Improves user experience in low-light conditions.
2. **Charts and Analytics**:
   - Income vs. Expense comparison.
   - Category-wise spending breakdown.

---

## **Backend Implementation**

### **Security**
- **Password Encryption**:
  - Passwords are encrypted using a salted hashing algorithm.
- **OTP Verification**:
  - Ensures only verified users can access the application.

### **Data Storage**
- **User Data**:
  - Stored securely with proper encryption.
- **Transaction Data**:
  - Captures amount, category, mode, type, and timestamps.
- **Category Data**:
  - Includes user-created categories and built-in categories.

---

## **Permissions**
1. **Notification**:
   - Used to send reminders and updates on transactions.
2. **SMS**:
   - Currently not in use; reserved for future features.

---

## **Future Enhancements**
1. **Subscription Restriction**:
   - Limit menu access based on subscription plans.
2. **Analytics**:
   - Advanced analysis of user transactions.
3. **Savings Management**:
   - Tools for setting and tracking financial goals.

---
