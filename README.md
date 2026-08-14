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

**Core Infrastructure Addons:**
These components handle networking, storage, and security within the cluster:
*   **Cert-Manager**: Certificate management for TLS (`apps/infrastructure/controllers/cert-manager`)
*   **External Secrets**: Securely inject secrets from external sources (`apps/infrastructure/controllers/external-secrets`)
*   **CloudNativePG**: Managed PostgreSQL database service (`apps/infrastructure/controllers/cloudnative-pg`)
*   **NGINX Ingress**: Load balancing and ingress controller for services (`apps/infrastructure/networking/nginx-ingress`)
*   **Metallb**: Network load balancer provider (`apps/infrastructure/networking/metallb`)
*   **External DNS**: Automated external DNS record management (`apps/infrastructure/networking/external-dns`)
*   **Longhorn**: Distributed block storage solution (`apps/infrastructure/storage/longhorn`)
*   **NFS Server Provisioner**: Network file system provisioner (`apps/infrastructure/storage/nfs-server-provisioner`)

**General Platform Utilities:**
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