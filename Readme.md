# DroneSmart: Smartphones Delivery System

![DroneSmart Logo](image\logo.png)

## Table of Contents

- [Introduction](#introduction)
- [Task Description](#task-description)
- [Requirements](#requirements)
  - [Functional Requirements](#functional-requirements)
  - [Non-functional Requirements](#non-functional-requirements)

---

## Introduction

Welcome to DroneSmart, an innovative project aiming to leverage drone technology for efficient and rapid delivery of small items. Just as mobile phones revolutionized personal communication, drones have the potential to transform the transportation landscape by enabling deliveries to remote or challenging locations.

Useful drone functions include delivery of small items that are urgently needed in locations with difficult access. Our project focuses on delivering smartphones to enhance accessibility and convenience.

---

## Task Description

In the DroneSmart project, we manage a fleet of 10 advanced drones, capable of carrying small loads. The primary cargo in our scenario is smartphones.

Each **Drone** has the following attributes:

- Serial Number (up to 100 characters)
- Model (Lightweight, Middleweight, Cruiserweight, Heavyweight)
- Weight Limit (500g maximum)
- Battery Capacity (percentage)
- State (IDLE, LOADING, LOADED, DELIVERING, DELIVERED, RETURNING)

Each **Smartphone** has the following attributes:

- Name (letters, numbers, '-', '\_')
- Weight
- Code (uppercase letters, underscore, numbers)
- Image (picture of the smartphone model)

We've developed a robust REST API that enables clients to interact with the drones, known as the **DroneSmart controller**. While the exact communication with the drones is not covered here, our API facilitates essential functions:

- Registering a drone
- Loading a drone with smartphone items
- Checking loaded smartphone items for a given drone
- Checking available drones for loading
- Checking drone battery level for a given drone

Feel free to interpret the design approach to best suit your implementation.

---

## Requirements

During the implementation of DroneSmart, please adhere to the following requirements:

### Functional Requirements

- User Interface is not required.
- Prevent drones from being overloaded beyond their weight capacity.
- Prohibit drones from entering LOADING state if the battery level is below 25%.
- Implement a scheduled task to monitor drone battery levels, generating history/audit event logs.

### Non-functional Requirements

- Input/output data must use JSON format.
- Ensure the project is buildable and runnable.
- Include a comprehensive README with build/run/test instructions. Feel free to use a local database (e.g., in-memory, containerized) for testing purposes.
- Preload necessary data into the database.
- While optional, we advise including JUnit tests.
- Your commit history can provide insights into your development process.

---

Feel free to contribute, enhance, or tailor DroneSmart as needed. We're excited to see how you'll tackle the challenges and create an efficient drone-powered smartphones delivery system! 🚁📱
