# 🚀 APT Discord Bot

<div align="center">

![Discord](https://img.shields.io/badge/Discord-Bot-7289da?style=for-the-badge&logo=discord&logoColor=white)
![Solana](https://img.shields.io/badge/Solana-Blockchain-9945ff?style=for-the-badge&logo=solana&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-Runtime-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-Language-f7df1e?style=for-the-badge&logo=javascript&logoColor=black)

**Discord bot for Solana**

</div>

---

## 📋 Table of Contents

- [🎯 Overview](#overview)
- [✨ Core Features](#core-features)
- [📊 Monitoring Services](#monitoring-services)
- [🔧 Utilities & Infrastructure](#utilities--infrastructure)
- [📝 Commands](#commands)
- [📸 Bot Demonstration](#bot-demonstration)
- [🏗️ Technical Architecture](#technical-architecture)
- [📈 Portfolio Highlights](#portfolio-highlights)

---

## 🎯 Overview

This Discord bot was developed to monitor various aspects of the Solana ecosystem. The project demonstrates implementation of real-time data processing, API integration patterns, and Discord bot architecture.

**Technologies Used:**
- Node.js with Discord.js library
- Multiple REST API integrations (SolanaTracker, Helius)
- WebSocket connections for real-time data
- JSON-based data persistence
- Proxy rotation and request management
- Rate limiting and caching systems

---

## ✨ Implementation Details

### Token Migration Monitoring
- SolanaTracker API integration for transaction data
- Custom filtering logic for specific program addresses (Pump.fun)
- Transaction threshold filtering (85+ SOL)
- Historical data comparison algorithms
- Market cap data aggregation and sorting

### Payment Verification System
- Automated DEX payment status checking
- Continuous monitoring with configurable intervals
- Multi-DEX compatibility through unified interface
- Notification system for payment status updates

### User Interface & Management
- Discord slash command implementation
- Channel configuration through user interactions
- Server-specific settings via JSON database
- Role-based permission system
- Automated welcome message system

---

## 📊 Services Architecture

### 🟢 Active Monitoring Services

#### BWE News Integration
- WebSocket connection implementation for real-time data
- Custom message filtering and processing
- Multi-channel distribution system

#### PrevRay Developer Tracking
- Token creator migration history analysis
- Pump.fun specific monitoring implementation

#### Trader Data Export
- CSV data export functionality
- Top 30 trader address monitoring
- Performance metrics calculation
- Rich embed data visualization

### 🔴 Experimental/Deprecated Features

#### Auto.fun Monitor
- Real-time token monitoring with proxy rotation
- Anti-detection techniques implementation
- Multi-threaded monitoring architecture
- Verified badge detection and filtering

#### Truth Social Monitor
- Multi-proxy system with endpoint rotation
- Adaptive HTTP client switching (native fetch, node-fetch)
- User agent rotation and header randomization
- Cookie session management
- Parallel account monitoring
- Anti-detection techniques and timing randomization

#### Telegram Integration
- Cross-platform notification system
- Group invitation automation

## 🔧 Technical Infrastructure

### Security & Performance Implementation
- Custom rate limiting with configurable thresholds
- Multi-proxy architecture for request distribution
- Dynamic header generation and user agent rotation
- Random interval scheduling for anti-detection
- Session management with cookie persistence
- Multiple HTTP client fallback methods

### Data Management Solutions
- JSON-based database with custom adapter pattern
- Time-based caching system with automatic expiration
- Batch processing for transaction data
- Memory management with automatic garbage collection

### Network & API Architecture
- Multi-API integration with SolanaTracker and Helius
- Automatic failover system between API endpoints
- Exponential backoff retry logic implementation
- HTTP connection pooling for efficiency

---

## 📝 Command Interface

### Migration Monitoring
- `!bonding <time>` - Token migration analysis (e.g., `!bonding 1h`, `!bonding 60m`)
- `!b <time>` - Shortened command variant
- `!bonding:compare <time>` - Historical comparison functionality

### Payment Verification
- `/dexcheck <address>` - DEX payment status verification
- `/dexmonitor <address>` - Continuous payment monitoring

### Data Analysis
- `/toptrader <address>` - Trader performance analysis with CSV export
- `/servers` - Server management (admin only)

### Configuration
- `/help` - Channel setup and configuration
- `/deploy` - Slash command deployment

---

## 📸 Bot Demonstration

### Migration Monitoring in Action
![Migration Monitoring](screenshots/bonding-command.png)
*Real-time token migration tracking with market cap analysis*

### DEX Payment Verification
![DEX Checker](screenshots/dex-checker.png)
*Automated payment status verification and monitoring*

### Trader Data Export
![Trader Export](screenshots/trader-export.png)
*CSV export functionality with performance metrics*

### News Integration
![BWE News](screenshots/bwe-news.png)
*Real-time news monitoring and filtering*

---

## 🏗️ Code Architecture

### Project Structure
```
├── bot.js                 # Discord client initialization and event handling
├── cmd/                   # Command handler modules
│   ├── bondings.js       # Migration tracking and analysis logic
│   ├── dexChecker.js     # Payment verification implementation
│   ├── dexMonitor.js     # Continuous monitoring system
│   ├── topTrader.js      # Trader analysis and CSV generation
│   └── slashCommands.js  # Discord slash command definitions
├── services/             # Background monitoring services
│   ├── bweNews.js       # WebSocket news monitoring
│   ├── prevRay.js       # Developer tracking service
│   └── autoFun.js       # Token monitoring (deprecated)
├── utils/               # Shared utility modules
│   └── rateLimiter.js   # Rate limiting implementation
└── db/                  # Data persistence layer
    └── jsonDb.js        # Database adapter and operations
```

### Key Implementations
- Concurrent processing for parallel API requests
- Smart caching with time-based invalidation
- Batch operations for efficient data processing
- Automatic memory cleanup and optimization

### Data Processing Pipeline
1. Input Processing → Command parsing and validation
2. Rate Limiting → Request throttling and user validation  
3. Data Retrieval → Multi-source API data aggregation
4. Analysis → Custom filtering and calculation algorithms
5. Output Generation → Discord embed formatting and delivery

---

## 📈 Technical Highlights

### Development Practices
- Modular architecture with separation of concerns
- Comprehensive error handling and graceful failure recovery
- Performance monitoring and memory usage optimization
- Input validation and secure API key management

### Advanced Features Implemented
- Context-aware caching with automatic invalidation
- API resilience with automatic failover
- Real-time integration using WebSocket and polling
- Stealth web scraping with anti-detection measures
- Multi-layered proxy rotation and user agent spoofing

### Problem-Solving Approaches
- Data consistency handling with API rate limits
- Scalable architecture for multiple Discord servers
- Reliable fallback mechanisms for critical operations
- Anti-detection evasion with proxy rotation and timing randomization
- Memory optimization with automatic cache management
- Cross-platform integration solutions

---

<div align="center">

**Invite to your server:**

https://discord.com/oauth2/authorize?client_id=1288990112893501540

</div>
