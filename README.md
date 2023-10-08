# ElasticSIEM Active Directory Simulation

![Project Image](https://github.com/ma7mouddiaa/SIEM-Detection-ActiveDirectory-Playground/blob/main/Untitled-1.png)

**Simulate, Detect, and Defend: A Comprehensive Active Directory Simulation with ElasticSIEM**

This cybersecurity project involves simulating an Active Directory (AD) environment with a domain controller (DC) and two Windows workstations. Utilizing the Elastic Stack SIEM (Security Information and Event Management) running on an Ubuntu server, the system is configured to its fullest potential. In addition, a Kali Linux machine is introduced to simulate various cyber attacks.

## Table of Contents

- [Introduction](#introduction)
- [Key Features](#key-features)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Simulated Attacks](#simulated-attacks)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Cybersecurity threats are evolving rapidly, necessitating effective tools and strategies to protect critical systems. This project focuses on creating a simulated Active Directory environment, a common target for attackers, and leveraging ElasticSIEM to monitor and detect potential threats. By simulating attacks and utilizing ElasticSIEM for detection and prevention, this project demonstrates robust cybersecurity measures for safeguarding an Active Directory environment.

## Key Features

- **Active Directory Simulation:** ![Static Badge](https://img.shields.io/badge/Active_Directory_Building-blue)
  - Domain Controller (DC) and two Windows workstations are configured to simulate a standard AD setup.
  - After setting up the AD, Started on the first layer of the ElasticStack which is log collection, it's done by installing sysmon on every machine and deploying agents (Winlogbeat for the DC, ElasticAgent "Fleet" for the workstations)

- **ElasticSIEM Integration:**
  - ElasticSIEM, part of the Elastic Stack, is deployed on an Ubuntu server to collect and analyze security events.
  - Data from various sources, including AD, is ingested into ElasticSIEM for comprehensive monitoring.

- **Attack Simulation:**
  - Kali Linux, a versatile penetration testing platform, is used to simulate cyber attacks on the AD environment.
  - Various attack scenarios are created to test the detection and prevention capabilities of ElasticSIEM.

## Project Structure

The project is structured as follows:

- `/AD_Simulation_ProjectFiles/`: Contains PowerShell scripts for setting up the Active Directory simulation.
- `/elasticsearch/`: Configuration files and instructions for deploying ElasticSIEM.
- `/kibana/`: Kibana configuration and setup details for visualization and analysis.

## Installation

Follow these steps to replicate the project environment and run the simulation:

1. **Setup Active Directory:**
   - Navigate to the `/AD_Simulation_ProjectFiles/` directory and run the provided PowerShell scripts to configure the AD environment.

2. **Deploy ElasticSIEM:**
   - Refer to the `/elasticsearch/` and `/kibana/` directories for instructions on setting up ElasticSIEM on an Ubuntu server.

3. **Simulate Attacks:**
   - Utilize Atomic Red to automate some attack and measure the detection rate
   - Utilize the Kali Linux machine to simulate various cyber attacks on the AD environment.

## Usage

1. **Accessing ElasticSIEM:**
   - Access the ElasticSIEM interface by navigating to the designated server IP and port (default: `http://server_ip:5601`).

2. **Monitoring and Analysis:**
   - Explore ElasticSIEM to monitor security events, analyze logs, and detect potential threats.

## Simulated Attacks ![Static Badge](https://img.shields.io/badge/Atomic_Red-Kali_linux-red)

Simulated attacks include but are not limited to:

- **Brute Force Attack:** Attempt to gain unauthorized access by trying multiple username and password combinations.
- **Malware Infection:** Simulate malware infiltration to test the system's response and detection capabilities.
- **Phishing Attempt:** Imitate a phishing attack to assess the system's ability to detect phishing attempts.

## Contributing

I welcome contributions! If you'd like to contribute to this project, please message me https://www.linkedin.com/comm/in/mahmoud-diaa-cybersamurai

## License

This project is licensed under the [MIT License](LICENSE).
