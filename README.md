# Virtual Reality CAPTCHA Authentication System

## Overview

The Virtual Reality CAPTCHA Authentication System is a security-oriented authentication platform designed to distinguish legitimate human users from automated bots through immersive virtual reality interactions.

Unlike traditional CAPTCHA systems that rely on text recognition or image selection, this project utilizes a VR puzzle-solving challenge combined with behavioral analysis techniques. The system evaluates user interaction patterns, completion time, retry attempts, and object placement accuracy to determine whether the participant is a genuine user or a potential automated attacker.

The project integrates Unity for the VR environment, Flask for backend services, and MySQL for secure data storage and analysis.

---

## Project Objectives

* Develop a secure VR-based CAPTCHA system.
* Differentiate between human users and automated bots.
* Analyze user behavior during puzzle interaction.
* Store and process challenge results securely.
* Provide a scalable cloud-based architecture.

---

## System Architecture

The system consists of three main layers:

### 1. VR Client Layer (Unity)

Responsible for:

* Presenting the VR CAPTCHA challenge.
* Handling user interactions.
* Tracking puzzle completion behavior.
* Collecting behavioral metrics.

### 2. Backend Layer (Flask API)

Responsible for:

* Receiving challenge submissions.
* Validating challenge tokens.
* Analyzing user behavior.
* Generating authentication decisions.
* Communicating with the database.

### 3. Database Layer (MySQL)

Responsible for:

* Storing challenge data.
* Recording user behavior metrics.
* Saving authentication results.
* Supporting future analysis and reporting.

### Architecture Flow

VR User

↓

Unity VR CAPTCHA Environment

↓

Behavior Tracking System

↓

Flask REST API

↓

Behavioral Analysis Engine

↓

MySQL Database

↓

PASS / FAIL / BOT_DETECTED Decision

---

## Technologies Used

### Frontend (VR Environment)

* Unity Engine
* C#
* XR Interaction Toolkit
* OpenXR

### Backend

* Python
* Flask
* Flask-Limiter
* Gunicorn

### Database

* MySQL
* MySQL Workbench

### Cloud Deployment

* Render (Backend Hosting)
* Railway (MySQL Database Hosting)

### Version Control

* Git
* GitHub

---

## Key Features

### VR CAPTCHA Challenge

Users must complete a virtual puzzle inside a VR environment.

### Behavioral Analysis

The system evaluates:

* Completion Time
* Retry Attempts
* Wrong Placements
* Interaction Consistency

### Bot Detection

Suspicious behavior triggers automatic bot classification.

### Security Validation

Includes:

* Token Validation
* Expiration Control
* Replay Attack Prevention

### Cloud-Based Infrastructure

Supports remote access through deployed backend and database services.

---

## Database Structure

### captcha_challenges

Stores generated challenge information.

### behavior_metrics

Stores behavioral data collected during puzzle interaction.

### captcha_results

Stores final authentication outcomes.

Authentication outcomes include:

* PASS
* FAIL
* BOT_DETECTED

---

## Authentication Logic

The system analyzes behavioral indicators to classify users.

### PASS

Assigned when:

* Puzzle is solved correctly.
* Interaction behavior appears human.
* Completion time falls within expected ranges.

### FAIL

Assigned when:

* User exceeds retry limits.
* Excessive placement errors occur.

### BOT_DETECTED

Assigned when:

* Completion time is unrealistically fast.
* Behavior strongly indicates automation.

---

## Testing and Evaluation

The system was evaluated using:

### Functional Testing

Verified:

* Challenge generation
* Puzzle interaction
* Result submission

### Integration Testing

Verified communication between:

* Unity
* Flask API
* MySQL Database

### Security Testing

Verified:

* Replay attack protection
* Token expiration handling
* Bot detection mechanisms

### Performance Evaluation

Metrics analyzed:

* Completion Time
* Behavior Score
* Retry Attempts
* Wrong Placements
* Decision Accuracy

---

## Deployment

### Backend

Hosted on Render.

### Database

Hosted on Railway MySQL.

### Source Code

Managed using GitHub.

---
## APK Download and Testing

A standalone APK version of the VR CAPTCHA Authentication System is available for testing purposes.

Users who own a compatible VR headset can download and install the APK directly on their device to experience the project and evaluate its functionality.

### Important Notice

This project is currently under active development and is intended for academic and research purposes only.

The current release should be considered a demonstration and testing version rather than a production-ready system.

At this stage:

* The project is not fully deployed for public use.
* Some features may still be under development or refinement.
* Cloud services and backend infrastructure are configured for project evaluation and demonstration purposes.
* Future updates may include additional security features, performance optimizations, and production deployment support.

We appreciate any feedback provided during testing and evaluation.

### Installation

1. Download the provided APK file.
2. Transfer the APK to your VR headset.
3. Enable installation from unknown sources if required.
4. Install the application.
5. Launch the VR CAPTCHA Authentication System and begin testing.

### Compatibility

The application has been developed and tested using Meta Quest VR devices. Compatibility with other VR platforms may vary.

---

## Future Enhancements

Potential future improvements include:

* Machine Learning-based behavioral classification.
* Advanced anomaly detection.
* Multi-factor VR authentication.
* Adaptive CAPTCHA difficulty.
* Real-time analytics dashboard.
* Enhanced user behavior profiling.

---

## Authors

This project was developed by:

Salamah Mohammad Obeidat
Ayham Ayman Al-Salahat
Abdallah Ali Talafha
Mohammad Ibrahim Al-Odeh

Department of Computer Science / Cybersecurity

Jordan University of Science and Technology (JUST)

Academic Year: 2025–2026

---

## License

This project is intended for educational and research purposes.
