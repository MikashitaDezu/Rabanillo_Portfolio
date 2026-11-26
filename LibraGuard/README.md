<p align="center">
  <img src="assets/logo.png" alt="LibraGuard logo" width="160">
</p>

<h1 align="center">LibraGuard</h1>

<p align="center">
  An IoT-integrated smart library management system.<br>
  RFID access control, noise monitoring, and book borrowing in one platform.
</p>

# LibraGuard

An IoT-integrated smart library management system that brings RFID access control, noise and crowd monitoring, book borrowing, and computer reservations into one platform. Built as a capstone project for BSIT at UEP Binalonan.

## Overview

Small school libraries often handle entry logs, borrowing, and computer use by hand or with tools that do not talk to each other. LibraGuard connects ESP32-based hardware at the door, the desk, and the reading area to a web and mobile app, so librarians see what is happening in one place and students can check their own records.

The system has three user roles (student, instructor, admin), and each role sees and does different things.

## System components

| Component | What it does |
|---|---|
| **LibraGate** (2 units) | ESP32 and RC522 RFID gates for entry and exit. Checks cards against a local whitelist and logs each pass. |
| **EchoGuard** | ESP32 noise monitor for the reading area. |
| **Librarian Desk Scanner** | RFID scanner at the librarian's desk. |
| **Computer Registry** | ESP32 and RC522 connected to the operator's PC over USB. Registers cards, confirms borrows and PC reservations, and issues one-day visitor passes. |
| **Web app** | Admin and user dashboards for access logs, borrowing, reservations, and registry tools. |
| **Mobile app** | Profile, borrowing records, gate logs, computer sessions, and account security. |

## Highlights

- **Works offline.** LibraGate firmware falls back from a portable router to campus WiFi, then stores scans on an SD card and uploads them when the connection returns.
- **Role-based access.** Students, instructors, and admins get separate permissions.
- **Hardware and software in one flow.** A card tap at a gate or registry shows up in the web app's logs and records.

## Tech stack

ESP32 (firmware) · RC522 RFID · SD card storage · React · Vercel · Render · Cloudflare

## My role

[Describe what you built, for example: hardware wiring, ESP32 firmware, system design, documentation.]

## Screenshots

[Add photos of the gate hardware and screenshots of the web and mobile apps.]
