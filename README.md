# PiNAS Webstack Template

A cleaned-up Docker and Caddy based webstack template for a Raspberry Pi home server.

This repository is based on my personal PiNAS setup. The goal is to run self-hosted services and static websites on a Raspberry Pi using Docker Compose, Caddy and mounted external storage.

## Features

- Caddy reverse proxy
- HTTPS-ready web server setup
- Docker Compose based service structure
- Example WebDAV container setup
- Static website hosting structure
- Raspberry Pi / Linux home-server oriented layout

## Example Services

- `caddy` — reverse proxy and web server
- `webdav` — Apache-based WebDAV service

## Example Folder Structure

```text
/mnt/web/
├── webstack/
│   ├── docker-compose.yml
│   └── caddy/
│       └── Caddyfile
└── sites/
    └── example-site/

/mnt/cloud/
└── webdav/
    ├── data/
    ├── var/
    └── conf/
        ├── webdav.conf
        └── .htpasswd

# PiNAS Webstack Template

A small Docker/Caddy based self-hosting template for a Raspberry Pi home server.

This project is based on my personal PiNAS setup, where I use a Raspberry Pi with external SSD/HDD storage for web hosting, WebDAV access and server experiments.

## Goals

- Self-host static websites on a Raspberry Pi
- Use Caddy as a reverse proxy and HTTPS web server
- Keep the setup simple and understandable
- Provide a clean template without private credentials or production data

## Planned Components

- Caddy reverse proxy
- Static website hosting
- Optional WebDAV service
- Optional Docker Compose setup
- Example folder structure for `/mnt/web`

## Example Folder Structure

```text
/mnt/web/
├── webstack/
│   ├── compose.yml
│   └── caddy/
│       └── Caddyfile
└── sites/
    └── example-site/
