# RoxilerSystems

This project is a Transactions Management System that allows users to view, search, and analyze transaction data. The system provides various features such as viewing transactions, generating statistics, and visualizing data through bar and pie charts.

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Technologies Used](#technologies-used)
4. [Getting Started](#getting-started)
5. [Backend API Endpoints](#backend-api-endpoints)


## Introduction

The Transactions Management System is designed to facilitate the handling and analysis of transaction data. Users can interact with backend API endpoints to view, search, and visualize transaction information.

## Features

- View a paginated list of transactions.
- Search transactions based on keywords or month.
- Generate statistics for a selected month, including total sale amount, total sold items, and total not sold items.
- Create a bar chart showing the distribution of transaction amounts within specified price ranges.
- Show a pie chart illustrating the distribution of items across different categories.

## Technologies Used

- Node.js
- Express.js
- MongoDB

## Getting Started

### Backend Setup

```bash
# Clone the repository
git clone https://github.com/your-username/your-repo.git

# Navigate to the backend directory
cd Backend

# Install dependencies
npm install

# Start the backend server
npm start
```

## Backend API Endpoints
### 1. Initialize Database

- **Url:** http://localhost:8000/
- **Method:** POST
![Screenshot (269)](https://github.com/rachit3014/BACKEND-ASSIGNMENT/assets/84663169/7386c716-5fdf-443e-bf68-13a612eb89a8)

### 2. List Transactions

- **Url:** http://localhost:8000/transaction?keyword={}&month={}&page={}
- **Method:** GET
- **Parameters:**
  - `month` (string): Selected month (e.g., '03' for March)
  - `keyword` (string): Search query for filtering transactions
  - `page` (number): Current page for pagination
    
![Screenshot (266)](https://github.com/rachit3014/BACKEND-ASSIGNMENT/assets/84663169/916dd753-e827-47c8-9170-66b191a2019a)

### 3. Transaction Statistics

- **Url:** http://localhost:8000/statics?month={}
- **Method:** GET
- **Parameters:**
  - `month` (string): Selected month
![Screenshot (265)](https://github.com/rachit3014/BACKEND-ASSIGNMENT/assets/84663169/991793d0-c823-4605-a02e-2373e032f492)

### 4. Bar Chart Data

- **Url** http://localhost:8000/chart?month={}
- **Method:** GET
- **Parameters:**
  - `month` (string): Selected month
![Screenshot (267)](https://github.com/rachit3014/BACKEND-ASSIGNMENT/assets/84663169/350d2b72-5ec1-45ea-a715-812f14a2c0fe)

### 5. Pie Chart Data

- **Url** http://localhost:8000/piechart?month={}
- **Method:** GET
- **Parameters:**
  - `month` (string): Selected month
![Screenshot (268)](https://github.com/rachit3014/BACKEND-ASSIGNMENT/assets/84663169/f98f04f3-98a5-4fe4-8b60-1fd739c1c4cf)


