# <img src="https://github.com/AI-Kajee/APDS7311_POE_Pancakes/blob/main/Images/compass.png" alt="Visual Studio Code" width="100" height="100">  Atlas Trust
---
# Table of Contents

1. [Overview](#overview)
2. [Features](#features)
    - [Login and Register](#login-and-register)
    - [User Dashboard](#user-dashboard)
    - [Payment Page](#payment-page)
    - [View Payments Page](#view-payments-page)
3. [Security Implementations](#security-implementations)
    - [SSL Certificates](#ssl-certificates)
    - [Prevention Against SQL Injection and Session Jacking](#prevention-against-sql-injection-and-session-jacking)
    - [XSS and Clickjacking Protection](#xss-and-clickjacking-protection)
    - [DDoS Protection](#ddos-protection)
    - [Sensitive Data Encryption](#sensitive-data-encryption)
4. [Software and Tools](#software-and-tools)
5. [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)
6. [API Testing](#api-testing)
7. [CI/CD Pipeline](#cicd-pipeline)
8. [Contributors](#contributors)
9. [License](#license)
10. [Code Attribution](#code-attribution)

---
### Youtube Demo
Click on the thumbnail below to watch our prototype run through.
[![Watch the video](https://github.com/AI-Kajee/APDS7311_POE_Pancakes/blob/main/Images/Black%20and%20White%20Simple%20Gaming%20YouTube%20Thumbnail.png)](https://youtu.be/-FJ6O3bWa0E)
---

## Overview

Welcome to the **Atlas Trust** project repository. Our team has designed and developed a secure and user-friendly website for an international bank. The website serves as the digital front for the bank, ensuring the safe transfer of sensitive customer data and secure transactions. 

At **Atlas Trust**, we prioritize security above all else, compliance, and performance, embedding robust **DevSecOps** practices into every phase of the project. Our approach integrates security seamlessly into development and operations, from automated testing to continuous monitoring, ensuring that potential vulnerabilities are addressed proactively. 

By leveraging modern technologies such as **React** and adhering to best security standards, we aim to deliver a highly reliable, scalable, and secure platform that meets the financial institution's requirements for secure data handling and exceptional user experience.
Your Data is safe with us.

---

## Features

The **Atlas Trust** website for the international bank includes the following key features:

- **Login and Register**: Users can securely create an account and log in to access their personalized dashboard, utilizing strong authentication methods to safeguard user credentials.

- **User Dashboard**: Once logged in, users are presented with a dashboard where they can view their account details, recent transactions, and other banking services. The dashboard provides a clean and intuitive interface for managing their banking needs efficiently.

- **Payment Page**: The payment page allows users to send money in various currencies. Users can choose from multiple currencies and are required to enter the recipient's **SWIFT code** for international transfers, ensuring compliance with international banking standards. This feature offers a secure and flexible solution for conducting cross-border transactions.

- **View Payments Page**: The user is also able to view all payments that they made on **Atlas Trust**

---


## Security Implementations

### SSL Certificates
- **SSL Implementation:** Both frontend and backend are secured with SSL certificates to encrypt data in transit.
- **MitM Attack Mitigation:** Uses asymmetric cryptography to protect data.
- **HTTPS Upgrade:** Ensures secure data transmission.

### Prevention Against SQL Injection and Session Jacking
- **Bcrypt:** Hashes passwords and sensitive info before storing in MongoDB.
- **Mongo-Sanitize:** Prevents NoSQL injection by sanitizing user inputs.
- **Secure Session Management:** Uses `HttpOnly` and `Secure` cookie flags.

### Cross-Site Scripting (XSS) and Clickjacking Protection
- **xss-clean Middleware:** Sanitizes inputs from POST bodies, query parameters, and URLs.
- **Helmet Middleware:** Sets HTTP security headers, including `X-Frame-Options` and `Strict-Transport-Security`.

### DDoS Protection
- **Rate Limiting:** Controls request rates using `express-rate-limit` to prevent DDoS attacks.

### Sensitive Data Encryption
- **Crypto for Payment Data:** Encrypts and decrypts sensitive payment info using a secure key stored in an environment file (.env) along with the Mongo URL.

For additional details, refer to our Word document: [APDS Pancakes Part 2](https://github.com/AI-Kajee/APDS7311_POE_Pancakes/blob/main/APDS_Pancakes_Part%202.docx)

--- 



## Software and Tools

<p align="center">
  <img src="https://github.com/AI-Kajee/APDS7311_POE_Pancakes/blob/main/Images/Visual%20Studio%20Code.jpeg" alt="Visual Studio Code" width="80" height="80">
  <img src="https://github.com/AI-Kajee/APDS7311_POE_Pancakes/blob/main/Images/React.js_Readme.jpg" alt="React" width="80" height="80">
  <img src="https://github.com/AI-Kajee/APDS7311_POE_Pancakes/blob/main/Images/MONGODBIMAGE.jpeg" alt="Mongo" width="100" height="80">
  <img src="https://github.com/AI-Kajee/APDS7311_POE_Pancakes/blob/main/Images/Figma_%20The%20Collaborative%20Interface%20Design%20Tool.jpeg" alt="Figma" width="80" height="80">
  <img src="https://github.com/AI-Kajee/APDS7311_POE_Pancakes/blob/main/Images/10%20Canva%20Magic%20Tricks%20That'll%20Save%20You%20100's%20of%20Hours%20%C2%BB%20Smartiac.jpeg" alt="Canva" width="100" height="80">
  <img src="https://github.com/AI-Kajee/APDS7311_POE_Pancakes/blob/main/Images/Google%20Ai%20Gemini%20Logo%20PNG%20vector%20in%20SVG%2C%20PDF%2C%20AI%2C%20CDR%20format.jpeg" alt="Gemini" width="80" height="80">
  <img src="https://github.com/AI-Kajee/APDS7311_POE_Pancakes/blob/main/Images/Top%205%20Postman%20Courses%20for%20Java%20Web%20Developers%20and%20API%20Testers%20in%202024%20-%20Best%20of%20Lot.jpeg" alt="Postman" width="100" height="80">
  <img src="https://github.com/AI-Kajee/APDS7311_POE_Pancakes/blob/main/Images/A%20Beginners%20Guide%20to%20CI_CD%20with%20GitHub%20Actions.jpeg" alt="GitHub Actions" width="100" height="80">
  <img src="https://github.com/AI-Kajee/APDS7311_POE_Pancakes/blob/main/Images/CircleCI%20Logo%20-%20PNG%20Logo%20Vector%20Brand%20Downloads%20(SVG%2C%20EPS).jpeg" alt="CircleCI" width="100" height="80">
  <img src="https://github.com/AI-Kajee/APDS7311_POE_Pancakes/blob/main/Images/Clean%20Code%20Programming%20Languages.jpeg" alt="SonarQube" width="100" height="80">
</p>

- **Visual Studio Code**: Our code editor of choice for writing and managing the React codebase, with extensions to enhance productivity and ensure code quality.
- **React**: The front-end library used to build a responsive, dynamic, and user-friendly interface for the website.
- **MongoDB**: Our database solution, providing a scalable and flexible NoSQL data storage for user accounts, transaction records, and other critical information.
- **Figma**: Used for planning and designing the prototype of the website.
- **Canva**: Used to alter the designs edit Images.
- **Gemini API**: Integrated to handle real-time currency conversions, allowing users to select different currencies for international transfers.
- **Postman**: Utilized for testing and testing API endpoints, ensuring that all functionality, including payments and user authentication, works as expected.

- **CI/CD Pipeline**:
  - **GitHub Actions**: Used to automate the development workflow, including testing, building, and deploying the application.
  - **CircleCI**: Incorporated to run automated tests and ensure continuous integration and delivery.
  - **SonarQube**: Employed for static code analysis to detect potential security vulnerabilities, bugs, and code quality issues.

---

## Getting Started

To run the **Atlas Trust** website locally, follow these steps:

### Prerequisites
- **Node.js** (v16 or later)
- **MongoDB** (Ensure MongoDB is installed and running locally or via a cloud service)
- **Git** (Optional but recommended)
  
### Installation

1. **Clone the repository**:
   ```bash
   [ git clone https://github.com/your-repo/atlas-trust.git](https://github.com/AI-Kajee/APDS7311_POE_Pancakes.git)
   ```

2. **Install dependencies**:
   Navigate to the project folder and install the necessary packages:
   ```bash
   npm install
   ```

3. **Set up environment variables**:
   Create a `.env` file in the root directory and configure your environment variables. Example:
   ```bash
   MONGO_URI=your_mongodb_connection_string
   GEMINI_API_KEY=your_gemini_api_key
   ```

4. **Start the backend server**:
   From the root directory, run the following command to start the backend:
   ```bash
   npm run dev
   ```
   This will start the backend server on `https://localhost:3001`.

5. **Start the frontend server**:
   Open a new terminal, navigate to the root directory, and run:
   ```bash
   npm start
   ```
   This will launch the frontend on `https://localhost:3000`.

### API Testing

- Use **Postman** to test API endpoints. The API base URL will be `https://localhost:3001/api/`.

### CI/CD Pipeline

- The CI/CD pipeline is set up using **GitHub Actions** and **CircleCI**, so changes pushed to the repository will automatically trigger testing, building, and deployment workflows.

---


### Contributors 

- Ameer Inder Kajee
- Nehal Singh
- Radhya Chinnapen

---

## License

This project is licensed under the **MIT License**. You are free to use, modify, and distribute the code, provided you include the original copyright notice and this permission notice in all copies or substantial portions of the software.

For more details, please refer to the [LICENSE](./LICENSE) file.

---

## Code Attribution
### Attribution

- The code snippet for implementing rate limiting using Express and `express-rate-limit` middleware is adapted from the Mozilla Developer Network's article on securing APIs with rate limiting.
  - Source: Mozilla Developer Network. (2023) *Securing APIs with express-rate-limit and express-slow-down*. Available at: [https://developer.mozilla.org/en-US/blog/securing-apis-express-rate-limit-and-slow-down/](https://developer.mozilla.org/en-US/blog/securing-apis-express-rate-limit-and-slow-down/) (Accessed: 8 October 2024).

- [Integration of Gemini AI in React](https://medium.com/@codewithadurintiashok/integration-of-gemini-ai-in-react-8872025088de) by Adurinti Ashok

- [How to Make React.js Use HTTPS in Development](https://medium.com/swlh/how-to-make-react-js-use-https-in-development-4ead560eff10) by SWLH

- [mongo-sanitize npm package](https://www.npmjs.com/package/mongo-sanitize) – A tool to sanitize MongoDB queries and prevent injection attacks.

- [express-brute npm package](https://www.npmjs.com/package/express-brute) – A rate-limiting middleware for Express to protect against brute-force attacks.



