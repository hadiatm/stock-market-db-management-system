# stock-market-database-management-system
Relational database system for stock trading, brokers, and portfolio management (MySQL + MS Access)


# Stock Market Trading and Portfolio Management System

A relational database system that models real-world stock trading — investors, brokers, stocks, transactions, and portfolios — built to replace error-prone manual tracking with a centralized, normalized database.

## Overview

Investors trade stocks through brokers, hold portfolios, and generate transaction histories. This project models those relationships with a 5-entity relational schema (Broker, Investor, Stock, TransactionRecord, Portfolio), normalized to Third Normal Form (3NF).

## Tools Used

- MySQL Workbench — schema design and SQL implementation
- XAMPP — local server management
- Microsoft Access — forms, reports, and relationship views
- draw.io — ER diagram design

## Key Features

- 5 normalized tables with primary/foreign key constraints for referential integrity
- SQL queries using JOINs, aggregate functions, GROUP BY, and sorting (e.g., total investment per investor, profit/loss per stock, most active broker)
- Indexing on InvestorID and StockID for query performance
- Stored procedures (`ShowAllBrokers`, `GetInvestorPortfolio`) for reusable logic
- A SQL view (`PortfolioSummary`) for simplified reporting
- Microsoft Access forms (Investor, Transaction) and grouped/aggregated reports
- Realistic sample data modeled on Pakistan Stock Exchange (PSX) listings

## Entity Relationships

- One broker manages several investors
- One investor performs several transactions
- One broker handles several transactions
- One stock is involved in several transactions
- Each investor has exactly one portfolio

## Files

- `database_project.sql` — full schema, sample data, queries, procedures, and views
- `DB_Project_Report.pdf` — full project report with ER diagrams and screenshots
