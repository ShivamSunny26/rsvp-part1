# 📂 Event Management Database

This part of the project focuses on designing and setting up the **database schema** for an Event Management Platform.  
The database supports user registrations, event creation, and RSVP tracking.

---

## ✨ Features
- Database schema with **3 main tables**: `Users`, `Events`, and `RSVPs`
- Relationship management using **foreign keys**
- Support for multiple RSVP statuses (`Yes`, `No`, `Maybe`)
- Compatible with **Supabase (Postgres)** and **MySQL**

---

## 🛠 Database Schema

### 1. Users
Stores information about registered users.

### 2. Events
Stores events created by users

### 3.RSVPs
Track which users RSVP to which events

## 🛠 Entity Relationship Diagram
Users (1) ────< Events (M)
Users (M) ────< RSVPs (M) >──── Events (M)
**Users -> Events** A user can create many events.
**Users <--> Events**: Many-to-Many relationship for event participation
