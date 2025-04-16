CS2202 Mini Project: Indian Railway Ticket Reservation System
===========================================================

Project Overview
---------------
This project implements a comprehensive Indian Railway Ticket Reservation System (IRCTC) that allows passengers to book, modify, and cancel train tickets. The system manages train schedules, seat availability, payments, and various other aspects of railway ticket booking.

`Drive Link containing CSV Files, Video Demo, Readme file, .SQL file :
https://drive.google.com/drive/folders/1yPFskGxgu_Gwmni4K4Oqfh2zkFO1-rjg?usp=sharing`

Key Features
-----------
- Passenger ticket booking for available trains
- Multiple class options (Sleeper, AC 3-tier, AC 2-tier, First Class)
- Seat availability and PNR status tracking
- Waitlist and RAC (Reservation Against Cancellation) system
- Train schedule and route management
- Cancellation and refund processing
- Concession categories for special passengers

Database Structure
----------------
The database consists of the following main tables:
1. passengers - Stores passenger information
2. trains - Contains train details
3. tickets - Manages ticket bookings
4. payment - Handles payment transactions
5. railwaystations - Stores station information
6. trainroutes - Manages train routes
7. seats - Tracks seat information
8. seatavailability - Manages seat availability
9. concessions - Handles concession categories
10. bookinghistory - Tracks booking history
11. cancellation_log - Records cancellations
12. coachconfig - Manages coach configurations
13. coachseatavailability - Tracks coach-wise seat availability
14. seatstatusbydate - Manages seat status by date

Setup Instructions
----------------
1. Prerequisites:
   - MySQL Server 8.0 or higher
   - Any MySQL client

2. Database Setup:
   a. Create a new database:
      ```sql
      CREATE DATABASE mini_irctc;
      USE mini_irctc;
      ```
   
   b. Import the database schema:
      - Connect to your MySQL server
      - Execute the command:
        ```sql
        source irctc_db_final.sql;
        ```
        

4. Running Queries:
   - Use the provided SQL queries to test the system
   - Common queries include:
     - PNR status tracking
     - Train schedule lookup
     - Seat availability check
     - Passenger list for specific trains
     - Waitlist status
     - Revenue reports
     - Cancellation records
