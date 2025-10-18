# Linux SSH Server Hardening Project

[cite_start]A project on hardening an OpenSSH server on Ubuntu[cite: 377, 408]. [cite_start]This includes configuring `sshd_config` (using `AllowUsers`) and UFW firewall rules to restrict access to specific users from designated IP addresses[cite: 382, 389].

## Project Overview

The goal of this project was to secure a Linux server's SSH access by implementing layered security policies. This moves beyond simple password authentication to a much more robust configuration.

## Key Security Configurations
* [cite_start]**User-Based Access Control:** Configured the `sshd_config` file to use the `AllowUsers` directive[cite: 389, 396]. [cite_start]This ensures that only explicitly named users (e.g., `samin-sh`, `sina-sh`) are permitted to log in via SSH[cite: 389].
* [cite_start]**IP-Based Access Control:** Restricted logins to only come from whitelisted IP addresses (both public and local)[cite: 389].
* [cite_start]**Firewall Rules:** Implemented `UFW` (Uncomplicated Firewall) rules to only allow incoming traffic on port 22 (SSH) from the specific whitelisted public IP[cite: 382].
* [cite_start]**Testing:** Verified the configuration by successfully logging in with an allowed user [cite: 419] [cite_start]and confirming that access was denied for unauthorized users (like `root`)[cite: 439].

## Key Technologies
* [cite_start]Linux (Ubuntu Server) [cite: 377, 408]
* [cite_start]OpenSSH Server (`sshd_config`) [cite: 371, 385]
* [cite_start]`UFW` (Firewall) [cite: 380]
* [cite_start]`AllowUsers` Directive [cite: 389]
* User Management

## Report
The full report, configuration steps, and verification screenshots are available in the `گزارش تمرین اصلی لینوکس.pdf` file in this repository.
