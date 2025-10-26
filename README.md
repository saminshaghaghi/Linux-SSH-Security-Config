# Linux SSH Server Hardening Project

A project on hardening an OpenSSH server on Ubuntu. This includes configuring sshd_config (using AllowUsers) and UFW firewall rules to restrict access to specific users from designated IP addresses.

## Project Overview

The goal of this project was to secure a Linux server's SSH access by implementing layered security policies. This moves beyond simple password authentication to a much more robust configuration.

## Key Security Configurations

* **User-Based Access Control:** Configured the sshd_config file to use the AllowUsers directive. This ensures that only explicitly named users (e.g., samin-sh, sina-sh) are permitted to log in via SSH.
* **IP-Based Access Control:** Restricted logins to only come from whitelisted IP addresses (both public and local).
* **Firewall Rules:** Implemented UFW (Uncomplicated Firewall) rules to only allow incoming traffic on port 22 (SSH) from the specific whitelisted public IP.
* **Testing:** Verified the configuration by successfully logging in with an allowed user and confirming that access was denied for unauthorized users (like root).

## Key Technologies

* Linux (Ubuntu Server)
* OpenSSH Server (sshd_config)
* UFW (Firewall)
* AllowUsers Directive
* User Management

## Report

The full report, configuration steps, and verification screenshots are available in the گزارش تمرین اصلی لینوکس.pdf file in this repository.
