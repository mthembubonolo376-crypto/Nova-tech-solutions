# Nova Tech Support Platform - System Specification

## 1. Overview

A full-stack business web platform built to support Small and Medium Enterprises (SMEs), Non-Governmental Organisations (NGOs), organisations, and educational institutions.

The system combines:
- A professional public website for marketing and credibility
- A client portal for bookings, invoicing, and service history
- An internal operations portal for administration, technicians, and reporting

The platform improves efficiency, transparency, and service delivery for both commercial and mission-driven organisations.

## 2. Target Users & Use Cases

### SMEs
- Manage client bookings and payments
- Track revenue and profitability
- Assign field technicians and manage work orders

### NGOs & Organisations
- Manage community service or outreach bookings
- Track service delivery and impact
- Maintain transparent records for reporting and compliance

### Schools & Educational Institutions
- Book maintenance or service requests
- Manage schedules and on-site visits
- Track service history and administrative workflows

## 3. Public Website

The public-facing website is the digital front door for professional and institutional clients.

### Core pages
- Home
- Services
- Blog / News
- Careers
- Testimonials
- Contact
- Legal pages (Terms & Conditions, Privacy Policy)

### Purpose
- Build credibility with organisations
- Clearly communicate service offerings
- Promote structured service bookings

### Recommended implementation
- Next.js for performance, SEO, and server-side rendering
- Responsive, mobile-friendly design
- Analytics integration (e.g. Google Analytics)

## 4. Client Portal

The client portal is designed for organisations and institutional customers.

### Authentication & Security
- Secure login system
- Role-based access control
- Organisation-level accounts
- Multiple users under one organisation
- Centralized booking, billing, and administration

### Booking System
- Service selection
- Date and time scheduling
- Terms and conditions acceptance
- Location capture (address and/or GPS)

### Payments
- Online payments via PayFast or Stripe
- Invoice-based payments for organisations
- Payment tracking and confirmation
- Auto-confirmation after verified payment

### Booking History
- Full service history for reporting and auditing
- Useful for NGOs and schools needing reliable records

### Notifications
- Booking confirmation emails
- Payment receipt emails
- Status update notifications
- Suggested providers: SendGrid or Mailgun

## 5. Admin & Technician Portal

The internal portal supports operations, job management, and reporting.

### Dashboard
- Total bookings
- Revenue tracking
- Gross profit calculations
- Service performance insights

### Booking Management
- Review and prioritize bookings
- Assign technicians by location or availability

### Technician Management
- Technician accounts
- Job assignment and updates
- Field service status tracking

### Job Tracking Lifecycle
- pending → confirmed → assigned → in progress → completed

### Financial Management
- Revenue vs expenses
- Gross profit visibility
- Financial reporting for SMEs and NGOs

## 6. Booking System

A structured booking workflow for institutional service delivery.

### Features
- Service selection
- Scheduled bookings
- Terms and conditions agreement
- On-site service handling

### Advanced logic
- Some services require physical visits
- Location data is required where applicable

## 7. Location Tracking

Location tracking is critical for on-site services.

### Basic functionality
- Store physical address details

### Advanced functionality
- Capture GPS location with user permission
- Map integration (e.g. Google Maps API)
- Optimize technician dispatch

## 8. Payment System

Supports both instant online payments and invoice workflows.

### Features
- PayFast or Stripe integration
- Invoice generation and delivery
- Backend payment verification
- Auto-confirmation of bookings after payment

## 9. Backend & Database

### Backend
- Node.js with Express

### Database
- PostgreSQL

### Key capabilities
- Multi-organisation support
- Secure data handling
- Scalable architecture

## 10. Additional System Requirements

### Multi-Tenant Support
- Each SME, NGO, or school has isolated data access
- Clear separation of organisation data

### Reporting & Transparency
- Downloadable reports in PDF or CSV
- NGO reporting, school administration, and audits

### Invoices & Receipts
- Automatically generated documents
- Essential for accounting and organisational workflows

### Security
- Strong authentication and session handling
- Role-based permissions
- Data protection compliance (POPIA-aware for South Africa)

### Mobile-Friendly Design
- Optimized for staff using phones in the field

### Performance
- Fast, reliable UX with Next.js

### Backup & Reliability
- Regular backups and high availability

### Legal Compliance
- Privacy Policy
- Terms & Conditions
- POPIA compliance
