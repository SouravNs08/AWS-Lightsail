# AWS-Lightsail
website on AWS -Lightsail
# Hosting a Website on AWS Lightsail

This guide will walk you through the steps to host a website on AWS Lightsail, including setting up the Lightsail instance, configuring your server, and deploying your website.

## Prerequisites

- AWS account.
- SSH client (e.g., PuTTY for Windows, Terminal for macOS/Linux).
- Basic knowledge of web server administration.

## Step-by-Step Guide

### 1. Create an AWS Lightsail Instance

1. **Log in to AWS Management Console:**
   - Go to [AWS Lightsail](https://lightsail.aws.amazon.com/).

2. **Create an Instance:**
   - Click on "Create instance".
   - Choose your instance location (preferably a region close to your target audience).
   - Select the platform (Linux/Unix).
   - Choose a blueprint (e.g., "OS Only" -> "Ubuntu").
   - Choose an instance plan (start with the lowest tier and scale as needed).
   - Name your instance.

3. **Create the Instance:**
   - Click the "Create instance" button.

### 2. Connect to Your Lightsail Instance

1. **Find your instance's public IP:**
   - Go to the Lightsail console, and you will see the public IP address of your instance.

2. **Connect via SSH:**
   - For macOS/Linux, open your terminal.
   - For Windows, use an SSH client like PuTTY.

   ```bash
   ssh -i /path/to/your/lightsail/key.pem ubuntu@your-lightsail-ip
