# OPSCPart2
Budget Tracker App
This is a Budget Tracker Android application that helps users manage their expenses, set budget goals, and track spending by categories. The app features user authentication, expense tracking with photos, category management, and comprehensive reporting 

Getting Started
User Authentication

Login with username and password

Basic validation for credentials

Category Management

Create custom categories for expenses

View all categories

Expense Tracking

Add expenses with date, time range, description, amount, and category

Optional photo attachment for receipts/proof

View all expenses with filtering by date range

Budget Goals

Set monthly minimum and maximum spending goals

Visual indicators for goal progress

Reporting

View total spending by category for selected periods

Access attached photos from expense list

Data Persistence

All data stored locally using Room Database

Photos stored in internal storage with references in database

Technical Implementation
Architecture
MVVM (Model-View-ViewModel) pattern

Repository pattern for data access

Single Activity with multiple Fragments

Language Used
Kotlin

Android Jetpack Components:

Room Database

ViewModel

LiveData

Navigation Component

CameraX for photo capture

Glide for image loading

Database Schema
User table (id, username, password)

Category table (id, name, userId)

Expense table (id, date, startTime, endTime, description, amount, categoryId, userId, photoPath)

BudgetGoal table (id, userId, minGoal, maxGoal, month, year)

Screens
Login Screen

Username and password fields

Login button

Main Dashboard

Current month's spending summary

Progress toward budget goals

Quick actions to add expense/view reports

Categories Screen

List of all categories

Add new category option

Add Expense Screen

Form with all expense fields

Photo capture/selection option

Category dropdown

Expense List Screen

Filter by date range

List of all matching expenses

Tap to view details/photo

Reports Screen

Spending by category chart

Date range selector

Total amounts per category

Clone the repository

Open project in Android Studio

Build and run on emulator or physical device

Testing Credentials

Username: user1

Password: password1 Known Limitations
No user registration flow (predefined users only)

Basic photo handling without advanced editing

No cloud sync/backup functionality

Simple reporting without export options

Future Enhancements
Add user registration

Implement data export (CSV/PDF)

Add recurring expenses feature

Dark mode support

