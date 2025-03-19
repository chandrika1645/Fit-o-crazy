# Fit-o-cracy

- A fitness website that uses Open AI to assess the user’s fitness level and provide personalized 
recommendations for diet and exercise.
- Implemented a BMI calculator that takes the user’s input on height, weight, age, and gender and displays the 
optimal range for their body type.
- Integrated Open AI with the website to generate custom diet plans and workout routines based on the user’s 
fitness goals, preferences, and availability.
- Utilized MongoDB, Node.js, Vite.js, and Open API to create a responsive, user-friendly, and secure web 
application.


# Images

<img src="https://raw.githubusercontent.com/chandrika1645/Fit-o-crazy/main/assets/screenshots/home-page.png" width="500">

<img src="https://raw.githubusercontent.com/chandrika1645/Fit-o-crazy/main/assets/screenshots/mongo-users.png" width="500">

<img src="https://raw.githubusercontent.com/chandrika1645/Fit-o-crazy/main/assets/screenshots/registration-form.png" width="500">

<img src="https://raw.githubusercontent.com/chandrika1645/Fit-o-crazy/main/assets/screenshots/generate-plan.png" width="500">

<img src="https://raw.githubusercontent.com/chandrika1645/Fit-o-crazy/main/assets/screenshots/generate-plan-continue.png" width="500">

<img src="https://raw.githubusercontent.com/chandrika1645/Fit-o-crazy/main/assets/screenshots/diet-plan.png" width="500">

<img src="https://raw.githubusercontent.com/chandrika1645/Fit-o-crazy/main/assets/screenshots/diet-plan-continue.png" width="500">

<img src="https://raw.githubusercontent.com/chandrika1645/Fit-o-crazy/main/assets/screenshots/BMI-cal.png" width="500">

<img src="https://raw.githubusercontent.com/chandrika1645/Fit-o-crazy/main/assets/screenshots/calorie-cal.png" width="500">


## Table of Contents
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Usage](#usage)
- [API Reference](#api-reference)
- [Code Structure](#code-structure)
  
---

## Features
- Personalized diet and workout recommendations powered by OpenAI
- BMI calculator that provides ideal body type ranges based on height, weight, age, and gender
- Custom diet plans and workout routines tailored to users' fitness goals
- Secure data handling and user authentication
- Responsive and user-friendly design for easy navigation

---

## Tech Stack
- **Frontend**: HTML, CSS, Vite.js, JavaScript
- **Backend**: Node.js, OpenAI API
- **Database**: MongoDB

---

## Installation

### Clone the Repository
```bash
git clone https://github.com/harshagnihotri10/Fit-o-cracy.git
```

### Backend Setup
1. Navigate to the backend directory:
   ```bash
   cd server
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the backend server:
   ```bash
   npm start
   ```

### Frontend Setup
1. Navigate to the frontend directory:
   ```bash
   cd client
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the frontend server:
   ```bash
   npm start
   ```

---

## Usage

1. Register or log in to your account.
2. Enter your details such as height, weight, age, and gender into the BMI calculator.
3. Choose your fitness goal and preferences.
4. Get a personalized diet plan and workout routine based on your inputs.

---

## API Reference

### OpenAI Integration
- **POST** `/api/generate-plan`
  - Description: Generates a custom diet and exercise plan based on user inputs.
  - Request Body:
    ```json
    {
      "height": "175",
      "weight": "70",
      "age": "25",
      "gender": "male",
      "goal": "muscle gain"
    }
    ```

### BMI Calculation
- **POST** `/api/calculate-bmi`
  - Description: Calculates the BMI based on user inputs.
  - Request Body:
    ```json
    {
      "height": "175",
      "weight": "70",
      "age": "25",
      "gender": "male"
    }
    ```

---

## Code Structure
```md
server/: Node.js backend code
  - src/: API endpoints and business logic
    - routes/: API route handlers
    - models/: MongoDB schemas for users and fitness plans
    - controllers/: Functions for handling requests
    - services/: Interaction with OpenAI API
  - tests/: Unit and integration tests for backend services

client/: Frontend code (Vite.js, HTML/CSS)
  - public/: Static assets (images, icons)
  - src/: React components and frontend logic
    - components/: Reusable UI components
    - services/: API calls to backend
  - App.js: Entry point for the React app

config/: Environment variables and configuration files
README.md: Project documentation
```

---



