Smart Campus Helpdesk API
Backend Project Assignment
📌 Project Overview

The Smart Campus Helpdesk API is a backend RESTful application built using Django and Django REST Framework.
It allows students to raise campus-related issues (tickets) and enables administrators to manage them efficiently.

This project demonstrates core backend concepts such as authentication, CRUD operations, filtering, pagination, and clean API design.

🎯 Objective

To implement a scalable and well-structured backend system using Django that supports:

Secure authentication

Ticket management

Efficient data querying

Professional project organization

🛠 Tech Stack

Backend Framework: Django, Django REST Framework

Database: PostgreSQL

Authentication: JWT (JSON Web Tokens)

API Testing: Postman

🚀 Core Features

Django project & app setup

PostgreSQL database integration

Ticket management system (CRUD)

JWT-based authentication

Admin session-based login

Pagination for ticket listing

Filtering by category & status

Ordering by priority & creation date

Search by title or description

Redis-ready caching structure (future enhancement)

📦 Ticket Data Model
Field	Type
id	AutoField
title	CharField
description	TextField
category	classroom / hostel / network
priority	low / medium / high
status	open / in-progress / closed
created_at	DateTimeField
updated_at	DateTimeField
🔐 Authentication Flow

User logs in with username & password

JWT access and refresh tokens are generated

Access token is sent in the Authorization header

Admin users can also authenticate via Django admin session

🔗 API Endpoints
Authentication

POST /api/token/ – Login

POST /api/token/refresh/ – Refresh access token

Tickets

POST /tickets/ – Create a ticket

GET /tickets/ – List tickets

GET /tickets/<id>/ – Ticket details

PATCH /tickets/<id>/ – Update ticket status

DELETE /tickets/<id>/ – Delete ticket

📄 Ticket Listing Flow

Apply filtering (category, status)

Apply ordering (priority, created_at)

Apply pagination

Return paginated response

🧠 Redis (Future Enhancement)

Redis will be used to cache the ticket listing API

Cache will be cleared on create/update/delete operations

Not implemented in current version

✅ Testing

APIs tested using Postman

Screenshots of responses included in submission

📁 Submission Notes

Complete Django project folder included

PostgreSQL used as the database

Code is clean, readable, and well-commented

Project structure follows best practices

👩‍💻 Author

Muskan Dhawan
Backend Developer | Django REST Framework
