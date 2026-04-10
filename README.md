# hotel-buhara-booking-system
A full-stack hotel website and booking management system featuring dynamic pricing, multi-language support, automated email notifications, and an admin dashboard.
# Hotel Buhara - Website & Booking System

A comprehensive, full-stack hotel website and booking management platform designed for Hotel Buhara. This system provides a seamless experience for guests while offering powerful backend tools for hotel staff to manage bookings, pricing, and daily operations.

## 🌟 Key Features

### Guest Experience
* **Real-Time Booking:** Availability checks and booking submissions with instant confirmation references.
* **Multi-Language Support:** Full translation support for English, Turkish, German, and Italian.
* **Dynamic Pricing Calculator:** Calculates base rates, seasonal multipliers, last-minute deals, and promo codes.
* **Rich Frontend Experience:** Showcases 8 distinct room types, amenities, guest reviews, and a live chat widget.
* **Automated Communications:** Check-in reminders, review requests, and WhatsApp Business integration.

### Admin & Staff Management
* **Secure Admin Dashboard:** Centralized hub for managing bookings, pricing, and system settings.
* **Booking Modifications:** Capability to look up bookings, change dates, switch room types, or process cancellations.
* **Staff Task Management:** Assign daily tasks, update task statuses, and view shift schedules.
* **Analytics & Logging:** Tracks login attempts, booking timestamps, contact submissions, and email/WhatsApp logs.

### Technical Highlights
* **Security First:** Implements CSRF protection, input sanitization, rate limiting, and unauthorized API blocking.
* **Data Persistence:** Local JSON storage (`/storage/bookings.json`) with CSV export capabilities.
* **Responsive Design:** Fully optimized for mobile and desktop viewing (iOS/Android Safari, Chrome, Firefox, Edge).
* **RESTful API Architecture:** Clear endpoints for authentication, contacts, bookings, and availability checks (e.g., `POST /bookings`, `GET /availability`).

## 📂 System Architecture & Technologies

* **Frontend:** HTML5, CSS3, JavaScript (Responsive, touch-friendly design).
* **Backend API:** PHP (`api/index.php`).
* **Storage:** JSON-based file storage structure.
* **Email System:** SMTP integration for automated mailing.

## 🚀 Deployment Guide

This project is optimized for deployment on standard hosting panels (like cPanel). 

1. **Upload Files:** Create a deployment ZIP and upload it to your server's `public_html` directory.
2. **Set Permissions:** Ensure file permissions are set correctly (644 for files, 755 for directories).
3. **Environment Setup:** Create your `.env` file on the server using `/.env.example` as a template. Configure:
   * `ADMIN_EMAIL` and `ADMIN_PASSWORD`
   * SMTP credentials
   * Optional: Stripe, Airtable, and WhatsApp keys
4. **Directory Preparation:** Ensure the `/storage/` directory is created and is writable by the server.

## 📖 Documentation

For further details on modifying or extending the system, please refer to the included documentation files:
* **API Endpoints:** `/API_DOCUMENTATION.md`
* **Full Deployment Steps:** `/DEPLOYMENT_GUIDE.md`
* **Testing & Verification:** `/TESTING_CHECKLIST.md`

---
*Developed for Hotel Buhara.*
