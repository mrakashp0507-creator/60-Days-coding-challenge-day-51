
# Mini Food Delivery Backend System

## Project Overview

A Python-based mini backend simulation of a food delivery
platform inspired by Swiggy and Zomato.

The system manages customers, restaurants, menu items,
orders, delivery partners, and delivery tracking.

## Core Modules

1. User Management
2. Restaurant Management
3. Menu Management
4. Order Management
5. Delivery Partner Management
6. Delivery Tracking

## Entity Relationships

- One User can place multiple Orders.
- One Restaurant can receive multiple Orders.
- One Restaurant can contain multiple Menu Items.
- One Order has one Delivery record.
- One Delivery Partner can complete multiple Deliveries
  over time.

## Order Lifecycle

PLACED
  -> ACCEPTED
  -> PREPARING
  -> READY_FOR_PICKUP
  -> PICKED_UP
  -> DELIVERED

Orders can be cancelled before pickup.

## Features

- User registration
- Restaurant registration
- Menu item management
- Order placement
- Automatic total calculation
- Order status validation
- Delivery partner assignment
- Delivery location updates
- Order history

## Architecture Decisions

- Object-oriented design
- Separate entity classes
- Central system coordinator
- In-memory dictionary storage
- Validated order state transitions
- Separate delivery tracking entity

## Technologies

- Python 3
- Object-Oriented Programming
- Dataclasses
- Python dictionaries

## How to Run

python food_delivery.py

## Limitations

This is an educational prototype.

- Data is stored in memory.
- No real payment gateway.
- No authentication.
- No actual GPS integration.
- No concurrent order processing.

## Future Enhancements

- PostgreSQL database
- REST API using FastAPI
- Customer authentication
- Payment integration
- Live GPS tracking
- Restaurant dashboard
- Delivery partner application
- Notification system
- Scalable microservices architecture
- 
