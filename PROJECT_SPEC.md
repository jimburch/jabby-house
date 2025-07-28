# Homelab Dashboard

This dashboard will serve as a home base for my Synology, which hosts \*arr services (Radarr, Sonarr, etc) in their own Docker containers. Each service uses a Cloudflare tunnel so I can access them remotely. `Cloudflared` is installed on a Raspberry Pi using the same network, which manages the tunnels, and will also host this dashboard.

### Stack

This dashboard uses:

- Vite
- TypeScript
- React
- Tailwind CSS

All UI components are built and stored in this project. I will not be using an external UI library.

### Features

The execution and layout will develop as we iterate on this dashboard, but the summary of desired goals and features are:

**Core Navigation & Access**
Unified App Launcher - Quick access tiles for all your apps with custom icons, descriptions, and direct links through your Cloudflare tunnels. Health Status Indicators - Real-time status badges showing if each service is online, offline, or experiencing issues. Search Integration - Universal search bar that can query across Radarr, Sonarr, and Plex simultaneously.
System Monitoring & Analytics

Resource Usage Dashboard - CPU, RAM, disk usage, and network activity for your Synology and individual Docker containers. Download Statistics - Charts showing download speeds, queue lengths, and completion rates over time. Storage Analytics - Disk space usage breakdown by media type, growth trends, and capacity planning alerts. Performance Metrics - Response times for each service, uptime statistics, and historical performance data.

**Media Management Features**
Recently Added Media - Unified feed showing latest movies and TV shows added across all services. Queue Management - Combined view of pending downloads, failed items, and manual intervention needed. Quality Profiles Overview - Quick reference for your quality settings across different apps. Release Calendar - Upcoming movie releases and TV episode air dates in a unified calendar view.

**Operational Intelligence**
Failed Downloads Dashboard - Centralized view of failed downloads with reasons and retry options. Indexer Health - Status of your torrent/usenet indexers with success rates and response times. Notification Center - Aggregated alerts from all services with customizable filtering and acknowledgment. Maintenance Reminders - Scheduled tasks, update notifications, and system maintenance alerts.

**Advanced Analytics**
Usage Patterns - When you download most content, peak usage times, and seasonal trends. Cost Analysis - Bandwidth usage costs, indexer subscription tracking, and storage expansion planning. Content Statistics - Library growth over time, most popular genres, quality distribution analysis. User Activity - If you share Plex access, viewing statistics and user engagement metrics.

**Automation & Control**
Bulk Operations - Mass actions across services like pausing downloads or updating quality profiles. Smart Alerts - Intelligent notifications based on patterns like unusual download failures or storage approaching limits. Quick Actions Panel - One-click operations like clearing completed downloads or refreshing metadata. Scheduled Operations - Visual timeline of automated tasks and their success/failure status.

**Security & Access Management**
Cloudflare Analytics - Traffic patterns, geographic access data, and security threat information for your tunnels. Access Logs - Who's accessing what services and when, with geographic insights. Security Dashboard - Failed login attempts, unusual access patterns, and tunnel health monitoring.
