# 🏠 Madhuri Niwash - Home Automation System

## Working Repos
 - git@github.com:madhuri-niwash/gateway.git (firwall certificates and all)
 - git@github.com:madhuri-niwash/router.git (routes requests based on domain and path)
 - git@github.com:madhuri-niwash/services.git (all services - admin, agreement, auth, cron, flag, github, iot, ip, misc, notify, power, wellknown)
 - git@github.com:madhuri-niwash/webapp.git (java based web app)
 - git@github.com:madhuri-niwash/eventbus.git (event bus to route all event to/from services controllers users-ui)
 - git@github.com:madhuri-niwash/ui.git (react ui app)

## Microcontrollers firmware repo
 - git@github.com:madhuri-niwash/sona.git (new controller to replace motor gate and rooftop)
 - git@github.com:madhuri-niwash/main-gate.git
 - git@github.com:madhuri-niwash/motor-controller.git
 - git@github.com:madhuri-niwash/rooftop-controller.git

## Utilities repo
 - git@github.com:madhuri-niwash/cicd.git (for my custom cicd)
 - git@github.com:madhuri-niwash/react-local-proxy.git (for local ui development)
 - git@github.com:madhuri-niwash/pcb.git (kicad pcb design)



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
