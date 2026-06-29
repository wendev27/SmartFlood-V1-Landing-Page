# SmartFlood V1 – Barangay Portal Prototype

## Overview

SmartFlood V1 – Barangay Portal Prototype is an early architectural prototype of the SmartFlood capstone project.

This repository was created to explore a deployment strategy where each barangay would have its own dedicated web application. The goal was to improve system organization and isolate access between different barangays while developing the early versions of SmartFlood.

Although this architecture was later replaced with a unified role-based system, this repository documents the initial design approach and the lessons learned during development.

---

## Purpose

The objective of this prototype was to:

* Explore separate deployments for individual barangays.
* Restrict users to viewing only the sensors assigned to their barangay.
* Prototype a secure monitoring dashboard for local government officials.
* Evaluate whether isolated deployments would improve security and system organization.

---

## Technologies Used

* Next.js
* React
* TypeScript
* MongoDB
* JavaScript / TypeScript

---

## Features Explored

* Barangay-specific dashboard
* Sensor filtering per barangay
* Restricted access to assigned sensor data
* Early authentication experiments
* Separate deployment architecture

---

## Architecture Concept

In this version, every barangay was intended to have its own deployment.

For example:

* Barangay Tanong officials could only view Sensor 1.
* Other barangays would only access the sensors assigned to their jurisdiction.

The objective was to provide strict separation between local government units and simplify access control during the early stages of development.

---

## Project Evolution

As SmartFlood continued to evolve, this architecture was replaced with a centralized system using Role-Based Access Control (RBAC).

Instead of maintaining multiple deployments for each barangay, a single application was developed where permissions determine which data a user can access.

This approach reduced maintenance complexity while still providing secure access to authorized users.

---

## Lessons Learned

This prototype helped me understand:

* Access control strategies
* Multi-tenant application concepts
* User authorization
* Dashboard design for different user roles
* Architectural trade-offs between multiple deployments and centralized RBAC

One important lesson from this prototype was that maintaining separate deployments for every barangay increases operational complexity. As the project matured, a centralized application with RBAC proved to be a more scalable and maintainable solution.

---

## Current Status

📦 Historical Prototype

This repository is preserved to document the early architectural decisions made during the development of SmartFlood. Although the deployment strategy changed, the concepts explored in this prototype influenced the design of later versions of the system.
