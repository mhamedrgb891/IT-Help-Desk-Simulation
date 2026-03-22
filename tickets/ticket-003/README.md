<p align="center">
  <a href="/tickets/ticket-002/README.md">⬅️ Previous (002)</a> • 
  <a href="/dashboard.md">🏠 Dashboard</a> • 
  <a href="/tickets/ticket-004/README.md">➡️ Next (004)</a>
</p>

# Ticket 003 - Slow Internet Connection

- **Submitted by:** Anna (Marketing)
- **Submitted on:** 2025-08-01
- **Priority:** 🟡 Medium
- **Status:** ✅ Resolved
- **Resolved by:** Mohamed Ragab (IT Support Technician)
- **Resolved on:** 2025-08-03

---

## Issue Description

> _Anna reports very slow internet speeds, especially when uploading files to the shared drive. Other applications such as email were also sluggish._

---

## Initial Diagnosis

1. Confirmed the user was connected to the office Wi-Fi with strong signal strength.
2. Performed a quick bandwidth test using **https://www.fast.com** — result showed **~400 kbps download**, confirming slowness.
3. Checked Task Manager → Performance tab → Network graph (no significant background network usage).
4. Verified no large file transfers or background updates in progress.

---

## Steps Taken to Resolve

1. **Verified Physical and Wireless Connectivity**

   - Signal strength was strong.
   - No loose cables or hardware issues detected.

2. **Checked for Local Network Congestion**

   - No heavy applications consuming bandwidth in Task Manager.
   - No other employees reported slow speeds at the same time.

3. **Performed Network Reset**

   - Opened **Settings** → **Network & Internet** → **Advanced network settings** → **Network reset**.
   - Confirmed the reset and allowed the system to reboot.
   - This reinstalled network adapters, reset the TCP/IP stack, and cleared the DNS cache.

4. **Re-tested Internet Speed**

   - Download speed returned to ~95 Mbps.
   - Upload speed also normalized.

---

## Final Resolution

> _The issue was caused by corrupted TCP/IP stack or cached network settings. A **Network Reset** restored normal internet speeds._

---

## Notes / Recommendations

- If the issue reoccurs, check for outdated network drivers.
- Train staff to run `ipconfig /flushdns` before performing a full reset.
- Keep Windows updated to maintain networking stability.

---

## Attachments

### 1 — Bandwidth Test Showing Slow Speed (~400 kbps)

![Bandwidth Test Showing Slow Speed](/assets/ticket-003/01-ticket-003-speed-check.png)

### 2 — Connectivity Status in Taskbar

![Connectivity Status in Taskbar](/assets/ticket-003/02-ticket-003-connectivity-check.png)

### 3 — Network Reset in Settings

![Network Reset in Settings](/assets/ticket-003/03-ticket-003-network-reset.png)

### 4 — Final Internet Speed Test (~95 Mbps)

![Final Internet Speed Test](/assets/ticket-003/04-ticket-003-final-speed-check.png)

---

<p align="center">
  <a href="/tickets/ticket-002/README.md">⬅️ Previous (002)</a> • 
  <a href="/dashboard.md">🏠 Dashboard</a> • 
  <a href="/tickets/ticket-004/README.md">➡️ Next (004)</a>
</p>
