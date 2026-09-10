# 🏠 Madhuri Niwash - Home Automation System

## Overview

Madhuri Niwash is a comprehensive home automation system designed to manage and control various smart devices in a residential environment. The system provides real-time monitoring, control, and automation capabilities for gates, motors, and other home appliances through a unified platform.

## Architecture

The system follows a microservices-based architecture with the following components:

### 1. Web Application (React)
- **Framework**: React 18 with Material-UI (MUI)
- **Features**: 
  - Real-time dashboard
  - Device management
  - User authentication
  - Event monitoring
  - WebSocket-based live updates

### 2. Backend Service (Spring Boot)
- **Framework**: Spring Boot 3.2.0
- **Language**: Java 21
- **Database**: MariaDB
- **Features**:
  - RESTful APIs
  - WebSocket server
  - JPA for data persistence
  - Spring Security for authentication
  - Real-time event bus

### 3. Event Bus Service (Go)
- **Language**: Go
- **Purpose**: Centralized event distribution
- **Features**:
  - WebSocket connections
  - Publish/Subscribe pattern
  - Persistent connections
  - Auto-reconnection

### 4. Cron Service (Go)
- **Language**: Go
- **Purpose**: Scheduled task execution
- **Features**:
  - Motor usage tracking
  - Limit enforcement
  - Scheduled operations

## Key Features

### 🔐 Authentication & Security
- Secure user authentication
- Role-based access control
- Token-based session management
- Admin and user roles

### 🚪 Gate Control
- Open/Close operations
- Person, bike, and car modes
- Scheduled closing
- Status monitoring
- Emergency stop functionality

### ⚙️ Motor Management
- Motor on/off control
- Usage tracking (24h and today)
- Daily limit enforcement
- Flat-wise motor control
- Usage history

### 📊 Real-time Monitoring
- Live event stream
- Device status updates
- Heartbeat monitoring
- Uptime tracking

### 🎯 Usage Analytics
- Motor usage by flat
- Duration tracking
- Limit monitoring
- Historical data

### 🔔 Notifications
- Real-time alerts
- Limit exceeded notifications
- System status updates

### ⚙️Events
 - event.motor
 - event.gate
 - event.rooftop
 - event.flag
 - event.trigger
 - event.data
 - event.notify
 - event.set

## Technology Stack

### Frontend
