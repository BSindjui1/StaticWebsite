# StaticWebsite

Static website deployed to AWS EC2 using GitHub Actions and Nginx (CI/CD pipeline project)



\## Overview

This is a \*\*static website\*\* deployed to an \*\*AWS EC2 instance\*\* using \*\*GitHub Actions\*\* and \*\*Nginx\*\*.  

The deployment is fully automated, meaning any change pushed to the `main` branch will update the website automatically.



---



\## Features

\- HTML/CSS static website

\- Automatic deployment via \*\*GitHub Actions\*\*

\- Hosted on \*\*AWS EC2\*\* with \*\*Nginx\*\* web server

\- Continuous integration and deployment (CI/CD) workflow

\- Ready for HTTPS with Let’s Encrypt (optional next step)



---



\## File Structure

StaticWebsite/

│

├── index.html

└── .github/

└── workflows/

└── deploy.yml



yaml

Copy

Edit



---



\## How it Works

1\. Code is pushed to the `main` branch.

2\. GitHub Actions workflow (`deploy.yml`) triggers.

3\. The workflow SSHs into the EC2 instance.

4\. Installs Nginx (if not already installed).

5\. Pulls the latest website code from GitHub.

6\. Updates permissions and reloads Nginx.

7\. Your website is live instantly.



---



\## Getting Started

\### Prerequisites

\- AWS EC2 instance (Ubuntu)

\- GitHub repository

\- GitHub Secrets set for:

&nbsp; - `EC2\_HOST` → Public IP of EC2

&nbsp; - `EC2\_USER` → `ubuntu`

&nbsp; - `EC2\_SSH\_KEY` → Contents of your `.pem` key



\### Deployment

After setting up secrets, simply push changes to the `main` branch, and the website will auto-deploy.



---



\## Author

\*\*Brandon Sindjui\*\* – DevOps \& Cloud Infrastructure Enthusiast

