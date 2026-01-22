## DNS & Connectivity Verification

After configuring DNS records, I verified name resolution and connectivity using standard networking tools.

- Used `ping` to confirm basic network reachability
- Used `nslookup` and `dig` to verify that the domain resolved to the expected public IP address

These checks confirmed that DNS resolution was functioning correctly, but they also highlighted that successful name resolution alone does not guarantee service availability.

---

## Troubleshooting & Validation

During setup, the domain resolved correctly but the web service was not initially accessible. This helped identify that the issue was not DNS-related, but related to network exposure.

Further investigation confirmed that inbound access depended on the correct security group configuration and open ports. Once HTTP/HTTPS ports were explicitly allowed and the web server was verified as running and listening, the service became accessible via the public IP and domain.

This reinforced the distinction between:
- DNS resolution (domain → IP)
- Network access control (security groups and ports)
- Application availability (NGINX running and reachable)

