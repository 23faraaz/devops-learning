# Networking Project

This project documents a hands-on networking exercise involving a cloud-hosted web server.

## Project Explanation
In this project, I deployed a basic public web service to understand how networking, DNS, and cloud infrastructure work together in practice.

I provisioned a cloud virtual machine (EC2) and configured network access using security groups, allowing inbound HTTP and HTTPS traffic. I then installed and configured NGINX to serve a web page.

Next, I configured DNS records to point a custom domain to the instance, enabling access via a human-readable domain name. Finally, I verified the full request flow by accessing the domain in a browser and confirming successful responses.

This project reinforced my understanding of how external traffic reaches cloud-hosted services through DNS, security controls, and application-level components.

