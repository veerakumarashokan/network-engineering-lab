# Lab 03: No Network – Adapter Disabled

## Overview
This lab demonstrates a scenario where a system has no network connectivity due to a disabled network adapter and how to diagnose and resolve the issue.

---

## Scenario
A system is unable to access the network or internet. The issue is caused by the network adapter being disabled.

---

## Initial State

System is connected and network is working.

- IP address is assigned  
- Internet connectivity is available  

![Initial Connectivity](01-initial-connectivity.png)

---

## Misconfiguration

The network adapter is manually disabled.

![Adapter Disabled](02-adapter-disabled.png)

---

## Issue Observed

After disabling the adapter:

- No IP address is shown in `ipconfig`  
- Network becomes unavailable  
- Ping to external IP fails  

![No Network](03-no-network.png)

---

## Troubleshooting

1. Checked IP configuration using `ipconfig`  
2. Observed missing network configuration  
3. Verified network adapter status in Network Connections  
4. Identified that the adapter is disabled  
5. Concluded disabled adapter as root cause  

---

## Resolution

Re-enabled the network adapter.

![Adapter Enabled](04-adapter-enabled.png)

---

## Verification

After enabling the adapter:

- IP address is assigned  
- Network connectivity is restored  
- Ping to external IP is successful  

![Connectivity Restored](05-connectivity-restored.png)

---

## Key Takeaway

- A disabled network adapter results in complete loss of connectivity  
- No IP address means no network communication  
- Always check adapter status as a first troubleshooting step  

---

## Interview Explanation

If a system has no network connectivity, I first check whether the network adapter is enabled. If it is disabled, I enable it and verify connectivity using tools like ipconfig and ping.
