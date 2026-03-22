<p align="center">
  <a href="#">⬅️ No previous</a> • 
  <a href="/dashboard.md">🏠 Dashboard</a> • 
  <a href="/tickets/ticket-002/README.md">➡️ Next (002)</a>
</p>

# Ticket 001 - Windows Audio Service Not Running

- **Submitted by:** Sarah (Marketing)
- **Submitted on:** 2025-07-31
- **Priority:** 🟠 Medium
- **Status:** ✅ Resolved
- **Resolved by:** Mohamed Ragab (IT Support Technician)
- **Resolved on:** 2025-08-01

---

## Issue Description

> _Sarah reported that she had no sound on her laptop. The speaker icon in the system tray showed a “X,” and hovering over it displayed the message: **"The Audio Service is not running."** This issue began after she force-shutdown the laptop while it was frozen._

---

## Initial Diagnosis

- Checked **Device Manager** → Audio drivers appeared installed but inactive.
- Verified that the **Windows Audio** service was stopped.
- Suspected cause: Service crash or failure to start after improper shutdown.

---

## Steps Taken to Resolve

### Step 1 — Check Audio Settings

- Right-clicked the sound icon → Selected **Troubleshoot sound problems**.
- Confirmed the troubleshooter detected “Audio service not running.”

---

### Step 2 — Start Audio Services Manually

- Pressed **Windows + R** → typed:

```
services.msc
```

- Located:
  - **Windows Audio**
- Set both to **Automatic (Delayed Start)** → Clicked **Start**.

---

### Step 3 — Restart Windows Audio from Command Prompt

- Opened **Command Prompt as Administrator** → ran:

```cmd
net stop audiosrv
net start audiosrv
```

- Ensured no error messages were returned.

---

### Step 4 — Test Sound Output

- Played a test sound via:
  - Control Panel → Sound → Playback → Speakers → Configure → Test
- Audio playback worked normally.

---

## Final Resolution

> _Restarting the Windows Audio services restored sound functionality. The issue was caused by the services failing to start after an improper shutdown._

---

## Notes / Recommendations

- Advise users to avoid force shutdown unless absolutely necessary.
- Consider setting a scheduled service health check via Group Policy for critical services.
- If issue reoccurs, reinstall audio driver via **Device Manager**.

---

## 📎 Attachments

### 1 — Showing disabled audio in Volume icon in the system tray

![Showing disabled audio in Volume icon in the system tray](/assets/ticket-001/01-ticket-001-system-tray-audio-icon-disabled.png)

### 2 — Disabled audio shown in control panel

![Disabled audio shown in control panel](/assets/ticket-001/02-ticket-001-control-panel-audio-disabled.png)

### 3 — Starting Windows Audio service in **services.msc**

![Starting Windows Audio service in Services](/assets/ticket-001/03-ticket-001-starting-audio-service.png)

### 4 — Proof of started Windows Audio service

![Proof of started Windows Audio service](/assets/ticket-001/04-ticket-001-started%20audio%20service.png)

### 5 — Restarting Windows Audio using CMD

![Restarting Windows Audio using CMD](/assets/ticket-001/05-ticket-001-disabling-enabling-audio-cmd.png)

### 6 — Audio hardware driver check in Device Manager

![Audio hardware driver check in Device Manager](/assets/ticket-001/06-ticket-001-audio-test.png)

### 7 — Testing sound output using control panel

![Testing sound output using control panel](/assets/ticket-001/07-ticket-001-audio-hardware.png)

### 8 — Showing enabled Volume icon in the system tray

![Showing enabled Volume icon in the system tray](/assets/ticket-001/08-ticket-001-system-tray-audio-icon-enabled.png)

<p align="center">
  <a href="#">⬅️ No previous</a> • 
  <a href="/dashboard.md">🏠 Dashboard</a> • 
  <a href="/tickets/ticket-002/README.md">➡️ Next (002)</a>
</p>
