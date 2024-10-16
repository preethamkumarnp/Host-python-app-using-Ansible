# Deploying Python Web Application with Ansible

This Ansible playbook automates the deployment of a Python web application using Flask, backed by a MySQL database. It streamlines the setup process by handling all necessary configurations, installations, and service management.

## Table of Contents

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Playbook Overview](#playbook-overview)
- [Installation](#installation)
- [Usage](#usage)
- [Example Inventory File](#example-inventory-file)
- [Configuration](#configuration)
- [Notes](#notes)
- [License](#license)

## Introduction

This playbook is designed for users who want to quickly deploy a Python web application with a MySQL backend on a Linux server. It sets up the required Python environment, installs necessary packages, and configures the MySQL database.

## Prerequisites

Before you begin, ensure you have the following:

- **Ansible**: Installed on your control machine.
  ```bash
  sudo apt-get install ansible

# Playbook Overview

This playbook automates the setup of a Python application with a MySQL database on a target system. Below is a detailed overview of the tasks performed by the playbook.

## Tasks Performed

1. **Enable Universe Repository**
   - Enables the Universe repository to access community-maintained software packages.

2. **Update APT Cache**
   - Updates the APT package cache to ensure the latest package versions are available for installation.

3. **Install Python 3 and Dependencies**
   - Installs Python 3 along with its necessary dependencies.

4. **Create a Virtual Environment**
   - Creates a virtual environment for the application to manage dependencies in isolation.

5. **Upgrade PIP**
   - Upgrades PIP within the virtual environment to the latest version.

6. **Install PyMySQL Package**
   - Installs the PyMySQL package, enabling interaction with MySQL databases using Python.

7. **Install MySQL Server and Client**
   - Installs both MySQL server and client for database management and connectivity.

8. **Manage MySQL Service**
   - Starts the MySQL service and ensures it runs on system startup.

9. **Create Databases**
   - Creates two databases: `bobdata` and `employee_db`.

10. **Create MySQL User**
    - Creates a MySQL user named `bob` with full privileges to manage the databases.

11. **Install Flask and Flask-MySQL**
    - Installs the Flask web framework and Flask-MySQL extension for web application development and MySQL connectivity.

12. **Copy Application Source Code**
    - Copies the application source code (`app.py`) to the target system.

13. **Start Flask Web Server**
    - Starts the Flask web server to host the application.

# Installation

## Clone the Repository

Replace `<repository-url>` with the actual URL of your repository.

```bash
git clone <repository-url>
cd <repository-directory>

