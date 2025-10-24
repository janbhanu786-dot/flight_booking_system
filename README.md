# flight_booking_system
A backend-to-frontend project that simulates a flight booking platform with flight search, dynamic pricing, concurrency-safe seat booking, and user interface integration.
## Overview
This project demonstrates the complete workflow of an airline booking system — from backend API design and database setup to frontend integration.
## It focuses on:
Building REST APIs for flight management
Implementing dynamic pricing based on demand and seat availability
Ensuring safe booking transactions with concurrency control
Providing an interactive frontend for users to search, book, and manage reservations
## Project Milestones
🧱Milestone 1: Foundational Database Setup
Objective: Set up and implement the core database for flights.
Tasks:
Design and implement database schema for flights.
Set up SQLite / PostgreSQL with sample or simulated data.
Practice SQL operations: INSERT, UPDATE, JOIN, transactions, and constraints.
Output:
Working database with populated flight data.
Verified SQL operations and constraints.
✈ Milestone 2: Flight Search & Dynamic Pricing Engine
Objective: Implement APIs for flight retrieval, search, and integrate a dynamic pricing engine.
Tasks:
1. Build REST APIs (Flask / FastAPI / Django) for:
Retrieving all flights
Searching by origin, destination, and date
2. Implement input validation and sorting (by price or duration).
3. Simulate external airline schedule APIs.
4. Design dynamic pricing logic using:
Remaining seat percentage
Time until departure
Simulated demand level
Base fare and pricing tiers
5. Integrate dynamic pricing with flight search API.
6. Build a background process to simulate demand and seat availability changes.
7. Store fare history for tracking price changes.
Output:
Working flight search API with live pricing updates.
Dynamic fare adjustments based on demand and time.
🧾 Milestone 3: Booking Workflow & Transaction Management
Objective: Implement the booking process with concurrency safety and confirmation tracking.
Tasks:
Design schema for bookings (flight_id, passenger_info, seat, status, price).
Develop a multi-step booking flow:
1. Flight & seat selection
2. Passenger info
3. Simulated payment (success/fail)
Generate unique PNR after successful booking.
Implement concurrency control using database transactions or locks.
Build booking cancellation and history retrieval endpoints.
Output:
End-to-end booking workflow.
Concurrency-safe seat reservations.
PNR generation and booking history tracking.
💻 Milestone 4: User Interface & API Integration
Objective: Build the frontend and connect all backend functionalities to deliver a full user experience.
Tasks:
Design UI using HTML/CSS/JS or React.
Integrate flight search and booking APIs into the frontend.
Display real-time dynamic prices in search results.
Build UI for the multi-step booking flow and PNR confirmation.
Generate and download booking receipts (PDF or JSON).
Final project polish and testing.
Output:
Fully functional frontend for booking simulator.
Seamless integration with backend services.
Downloadable booking receipts.
Usable, testable, and complete user experience.
## ⚙ Tech Stack
Layer	Technologies
Backend Framework	Flask / FastAPI / Django
Frontend	HTML / CSS / JavaScript / React
Database	PostgreSQL / SQLite
Language	Python 3
API Format	REST (JSON)
Tools	SQLAlchemy / Django ORM / Alembic
## 🌐 API Endpoints Overview
Method	Endpoint	Description
GET	/flights	Retrieve all flights
GET	/flights/search	Search flights by origin, destination, and date
POST	/booking	Create a new booking
POST	/payment	Simulate payment for booking
GET	/booking/{pnr}	Retrieve booking details
DELETE	/booking/{pnr}	Cancel booking
GET	/history	Retrieve booking history
## 🎨 Frontend Features
Responsive UI for flight search and booking
Dynamic fare updates in real time
Multi-step booking with confirmation tracking
PDF/JSON receipt generation
Interactive and user-friendly experience
## 🔮 Future Enhancements
Add real-world airline APIs for live flight data.
Implement user authentication (JWT).
Integrate email notifications for booking confirmation.
Include admin dashboard for analytics and management.
## 🧑‍💻 Author
Charitha Muppala

Guided by Springboard Mentor 564
## 📄 License
This project is licensed under the MIT License — feel free to use, modify, and share with attribution.
