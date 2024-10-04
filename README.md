# Stock Trading Bot Application

## Overview

<p>This is a backend application built with Node.js that simulates a basic trading bot for a hypothetical stock market. The bot continuously monitors stock price changes using mock data and executes trades based on predefined rules. It also tracks the bot's balance, shares owned, and profit/loss over time. The application logs trades and prints analytics in real-time.</p>


## Features

**1.Simulated Stock Prices:** The application fetches mock stock prices in real-time.

**2. Trading Logic:** Implements a simple strategy:

**a. Buy:** When the stock price drops by 2% from the last price.

**b. Sell:** When the stock price increases by 3% from the last price.

**3. Profit/Loss Tracking:** Tracks the bot's current balance, shares owned, and overall profit/loss.

**4. Logging:** Trades and analytics are logged in both the terminal and a tradeLog.txt file.

**5. Performance Analytics:** Includes metrics for total trades, profit/loss ratio, and overall performance.

## Technologies Used

**1. Node.js:** Backend framework.

**2. Express.js:** Web server framework.

## Installation

**1.Clone the repository:**

git clone https://github.com/Anjali9561Gupta/Trading-Bot-App-Nodejs-Assignment.git

cd stock-trading-bot

**2. Install dependencies:**

npm install

**3. Create .env file:**

Create a .env file in the root directory to define the environment variables. Example:

**4. PORT=3000**

**4. Run the application:**

npm start

The server will start running on http://localhost:3000.

