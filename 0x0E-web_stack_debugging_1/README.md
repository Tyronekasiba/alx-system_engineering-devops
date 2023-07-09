
# Web Stack Debugging #1

This repository provides information and instructions for debugging common web stack issues. The focus of this debugging exercise is to address the issue of an unrecognized Nginx service.

## Problem Description

When attempting to check the status of the Nginx service using the command `service nginx status`, an error message "nginx: unrecognized service" is displayed.

## Solution

To resolve the issue of an unrecognized Nginx service, follow these steps:

1. Check Nginx Installation:
   - Verify if Nginx is installed by running the command `nginx -v`.
   - If Nginx is not installed, install it using the appropriate package manager for your system. For example, on Ubuntu, use:
     ```
     sudo apt-get update
     sudo apt-get install nginx
     ```

2. Start Nginx Service:
   - Start the Nginx service using the command:
     ```
     sudo service nginx start
     ```

3. Verify Nginx Service Status:
   - Check the status of the Nginx service to ensure it is running without any errors:
     ```
     sudo service nginx status
     ```

4. Debugging Further:
   - If the issue persists, double-check the installation process and review the Nginx configuration files to ensure they are correctly set up.
   - Consider checking log files (`/var/log/nginx/`) for any error messages or relevant information that could assist in identifying and resolving the issue.

Remember to run the commands with appropriate privileges (e.g., using `sudo`) if required.

## Contributing

Contributions to this repository are welcome.
