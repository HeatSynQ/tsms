# TSMS - Tailor Shop Management System

A JavaFX-based desktop application for managing tailor shop operations, featuring role-based access control and file-based data persistence.

## Overview

TSMS is a management system built for tailor shops to efficiently handle customer orders, employee assignments, and order tracking. The application implements authentication system with distinct interfaces for administrators and employees.

## Features

### Admin Features
- **Order Management**
  - Create new customer orders
  - Update existing order details
  - Delete orders
  - View all orders details
  - Update order status (Complete/Incomplete)
  
- **Order Organization**
  - Sort orders by time
  - Sort orders by ID
  
- **Employee Assignment**
  - Assign orders to specific employees
  - Track employee workload

### Employee Features
- **Personal Dashboard**
  - View only assigned orders
  - Update status of personal orders
  - Track order completion
  
- **Smart Order Queue**
  - "Get Next" button to retrieve next order based on deadline
  - Deadline-based priority system
  - Focused work interface

### Security
- Role-based authentication (Admin/Employee)
- Login system
- User-specific data access

## Technology Stack

- **Java** - Core programming language
- **JavaFX** - GUI framework for desktop interface
- **File System (.txt)** - Custom file-based database implementation

## Data Architecture

The application uses a text file-based storage system:

- `userData.txt` - User credentials and authentication data
- `data.txt` - Master file containing all orders
- `[employee].txt` - Individual employee order files (e.g., `umar.txt`, `rafay.txt`)

Each employee has a dedicated file containing only their assigned orders, ensuring data isolation and efficient access.

## Technical Highlights

- **Multi-user system** with role-based access control
- **CRUD operations** for order management
- **Data persistence** through custom file handling
- **Sorting algorithms** for order organization
- **Business logic** implementation (deadline tracking, order assignment)
- **Clean separation** between admin and employee interfaces

## User Interface

### Admin Interface
- Comprehensive order listing
- Full CRUD functionality
- Order sorting controls
- Status management
- Employee assignment tools

### Employee Interface  
- Simplified, focused view
- Personal order queue
- Status update capabilities
- Deadline-based "Get Next" feature

## 📸 Screenshots

*Screenshots would be added here if available*

## 🔧 Setup & Installation

### Prerequisites
- Java JDK 11 or higher
- JavaFX SDK
- IDE with JavaFX support (Eclipse, IntelliJ IDEA, or VS Code with Java extensions)

### Running from Source

1. Clone the repository
```bash
git clone https://github.com/HeatSynQ/tsms.git
cd tsms
```

2. Ensure JavaFX is configured in your IDE

3. Run the main application file from `src/application/`

## 📝 Development Notes

This project was developed as a semester project to demonstrate:
- Object-oriented programming principles
- Desktop application development
- User authentication and authorization
- File I/O operations
- GUI design and user experience
- Business logic implementation

While the file-based storage is simple compared to modern databases, it effectively demonstrates understanding of data persistence, file handling, and CRUD operations.

## Future Enhancements

Potential improvements for this project could include:
- Migration to SQL database
- Report generation (PDF/Excel)
- Customer management module
- Invoice generation
- Data backup and recovery
- Search functionality
- Analytics dashboard

## Author

**HeatSynQ**