# NDatabase Connectivity Troubleshooting Guide

## Symptoms
- Cannot access network resources
- "Network unreachable" errors
- Intermittent connectivity

## Quick Checks

1. **Verify physical connection**

   ```bash
   # Check network interface status
   ip link show
   # or on Windows: ipconfig /all
ping 127.0.0.1  # Test loopback
ping <gateway-ip>  # Test gateway
nslookup google.com
# or: dig google.com
