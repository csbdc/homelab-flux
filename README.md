# Homelab Flux Deployment Guide

This repository contains configurations and source code for various services deployed within this homelab environment. The applications are organized into specific directories based on their function or origin.

## 🚀 Deployed Applications Overview

The following services are available in the `apps/` directory structure.

### 🏠 Home Services (User Facing)
These applications provide personalized services and media consumption features:
*   **Mealie**: Meal planning and recipe management (`apps/home/mealie`)
*   **Jellyfin**: Media server for streaming personal content (`apps/jellyfin`)
*   **Radarr / Sonarr / Bazarr**: Media collection tools for automatic organization (`apps/{radarr,sonarr,bazarr}`)
*   **Prowlarr / qbittorrent**: Indexing and download management utilities (`apps/{prowlarr,qbittorrent}`)
*   **Seerr**: Movie/TV show media frontend (`apps/seerr`)

### 🛠️ Infrastructure & Platform Services (Backend)
These services manage the underlying infrastructure and platform capabilities:
*   **Authentik**: Identity and access management system (`apps/authentik`)
*   **Harbor**: Private container registry (`apps/harbor`)
*   **Kube-Prometheus-Stack / Observability**: Monitoring and logging stack (`apps/{kube-prometheus-stack,observability}`)
*   **Metrics Server**: Provides basic resource metrics to Kubernetes (`apps/metrics-server`)
*   **Platform Utilities**: General purpose tools like `dispatcharr`, `ingest` (`apps/{dispatcharr,ingest}`)

### 💼 Productivity & Development Services
These applications focus on productivity, development, and data management:
*   **Household Budget Planner / Deposit Tracker**: Personal financial tracking apps (`apps/{household-budget-planner,deposit-tracker}`)
*   **Blueprints / Rust**: Project scaffolding/development tools (`apps/{blueprints,rust}`)
*   **Control**: Centralized control plane or orchestration tool (`apps/control`)

### 🎮 Misc Services
Miscellaneous applications:
*   **Game**: Game server or related utility (`apps/game`)
*   **Media / Playback**: General media handling services (`apps/{media,playback}`)