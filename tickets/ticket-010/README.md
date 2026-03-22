<p align="center">
  <a href="/tickets/ticket-009/README.md">⬅️ Previous (009)</a> • 
  <a href="/dashboard.md">🏠 Dashboard</a> • 
  <a href="/tickets/ticket-010/README.md">➡️ Last Ticket</a>
</p>

# Ticket 010 - VPN not connecting

- **Submitted by:** Lisa (Remote User)
- **Submitted on:** 2025-08-06
- **Priority:** 🔴 High
- **Status:** ⏳ In Progress
- **Handled by:** Mohamed Ragab (IT Support Technician)
- **Resolution Date:** —

---

## Issue Description

> Lisa reported being unable to connect to the company VPN while working from a public café. The VPN client repeatedly attempts to connect before timing out. Lisa confirmed internet access to other websites is working.

---

## Initial Diagnosis

- Verified Lisa’s credentials are active and not locked in Active Directory.
- Confirmed her VPN client version is up-to-date (Cisco AnyConnect v5.0).
- Reviewed VPN server logs — multiple failed connection attempts from Lisa’s IP, no authentication errors noted.
- Suspect possible **public Wi-Fi restrictions** (blocked VPN ports or protocols).

---

## Steps Taken So Far

1. **Connection Test:**  
   Guided Lisa to attempt connection from home network — VPN connected successfully. Confirms the issue is location-specific.

2. **Port/Protocol Verification:**  
   Verified VPN requires UDP port 500 and 4500 open for IPsec, or TCP 443 fallback. Informed Lisa to check with café staff about network restrictions.

3. **Alternate Connection Method:**  
   Provided instructions for switching VPN client to SSL/TCP mode to bypass potential UDP blocks. Testing pending.

4. **Ongoing Monitoring:**  
   Left ticket open to verify results after Lisa’s next attempt at the café.

---

## Final Resolution

> **Pending** — awaiting user confirmation after testing alternate connection method.

---

## Notes / Recommendations

- If public network blocks VPN, recommend using personal hotspot or a different location.
- Consider enabling “Always-On” VPN with automatic protocol switching for remote staff.
- Maintain documentation of VPN port requirements for end-users.

---

## Attachments

_(No screenshots collected yet — pending outcome of alternate connection test.)_

---

<p align="center">
  <a href="/tickets/ticket-009/README.md">⬅️ Previous (009)</a> • 
  <a href="/dashboard.md">🏠 Dashboard</a> • 
  <a href="/tickets/ticket-010/README.md">➡️ Last Ticket</a>
</p>
