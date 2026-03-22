<p align="center">
  <a href="/tickets/ticket-006/README.md">⬅️ Previous (006)</a> • 
  <a href="/dashboard.md">🏠 Dashboard</a> • 
  <a href="/tickets/ticket-008/README.md">➡️ Next (008)</a>
</p>

# Ticket 007 - Broken HDMI port

- **Submitted by:** John (Engineering)
- **Submitted on:** 2025-08-03
- **Priority:** 🟡 Medium
- **Status:** ✅ Resolved
- **Resolved by:** Mohamed Ragab (IT Support Technician)
- **Resolved on:** 2025-08-05

---

## Issue Description

> John reported that his external monitor was not displaying any output when connected to his laptop. The HDMI port on the laptop appeared physically loose, and the monitor was not detected in Windows display settings.

---

## Initial Diagnosis

- Connected a known working HDMI cable and verified that the external monitor worked with another laptop — eliminating the monitor and cable as the cause.
- Inspected John’s HDMI port physically and noticed movement when inserting the cable, indicating possible internal connector damage.
- Checked **Device Manager** → **Display adapters** and **Monitors**. No external display detected.
- Ran `dxdiag` to confirm only the internal display was recognized.

---

## Steps Taken to Resolve

1. **Test Alternate Video Output:**  
   Connected the external monitor via USB-C to HDMI adapter — display worked correctly, confirming the laptop’s GPU was functioning.

2. **Attempt Temporary HDMI Reseat:**  
   Powered off laptop, reinserted HDMI cable carefully — still not detected.

3. **Driver & Firmware Check:**

   - Updated GPU drivers using manufacturer’s software (Intel Graphics Command Center).
   - Installed pending Windows updates and rebooted.
   - Retested — no detection via HDMI.

4. **Escalate Hardware Issue:**  
   Logged hardware fault in asset management system and arranged for manufacturer warranty repair (HDMI port replacement).

5. **Interim Solution for User:**
   - Issued USB-C to HDMI adapter so John could continue working with his external monitor.
   - Documented adapter assignment in IT inventory.

---

## Final Resolution

The HDMI port was confirmed physically damaged and non-functional. A warranty repair request was submitted for port replacement. User was provided with a USB-C to HDMI adapter to maintain productivity until the repair is completed.

---

## Notes / Recommendations

- Recommend users avoid excessive force when connecting/disconnecting HDMI cables.
- Consider stocking spare USB-C to HDMI adapters for quick issue mitigation.
- During next hardware refresh, evaluate models with reinforced HDMI ports or alternate video output standards.

---

## Attachments

### 1 — Windows display settings showing no second monitor

![Windows display settings showing no second monitor](/assets/ticket-007/01-ticket-007-settings-display.png)

### 2 — Device Manager with only integrated monitor

![ Device Manager with only integrated monitor](/assets/ticket-007/02-ticket-007-device%20manager.png)

### 3 — Device Manager's display adapters

![Display Adapters](/assets/ticket-007/03-ticket-007-device-manager.png)

---

<p align="center">
  <a href="/tickets/ticket-006/README.md">⬅️ Previous (006)</a> • 
  <a href="/dashboard.md">🏠 Dashboard</a> • 
  <a href="/tickets/ticket-008/README.md">➡️ Next (008)</a>
</p>
