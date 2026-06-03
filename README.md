# Stock Market Trading System

A desktop-based stock market simulation built with Python, MySQL, and PySimpleGUI as a DBMS course project.

## Features

- User login and sign up
- View Nifty 50 stocks with price and % change
- Buy shares and track portfolio
- MySQL backend with relational schema

## Tech Stack

- Python 3
- MySQL
- PySimpleGUI
- mysql-connector-python

## Setup

**1. Install dependencies**
```bash
pip install mysql-connector-python PySimpleGUI
```

**2. Create the database**
```sql
CREATE DATABASE project1;
```

**3. Initialize tables and data (run once)**
```bash
python creatingTables.py
python insertingStaticData.py
python insertingDynamicData.py
```

**4. Run the app**
```bash
python loginpageGUI.py
```

## Database Schema

- `stock_info` — Nifty 50 stock data (LTP, open, % change)
- `user_info` — Registered users
- `portfolio` — User holdings with buy price and MTM value
