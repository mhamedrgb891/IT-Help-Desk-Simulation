<p align="center">
  <a href="/tickets/ticket-007/README.md">⬅️ Previous (007)</a> • 
  <a href="/dashboard.md">🏠 Dashboard</a> • 
  <a href="/tickets/ticket-009/README.md">➡️ Next (009)</a>
</p>

# Ticket 008 - Shared folder access denied

- **Submitted by:** Priya (Legal)
- **Submitted on:** 2025-08-02
- **Priority:** 🔴 High
- **Status:** ✅ Resolved
- **Resolved by:** Mohamed Ragab (IT Support Technician)
- **Resolved on:** 2025-08-02

---

## Issue Description

> _Priya reported she could not access the **Legal_2025** shared folder. She received an **"Access Denied"** message when attempting to open it from her mapped network drive. She confirmed she had access last week._

---

## Initial Diagnosis

- Confirmed Priya was connected to the corporate network by verifying VPN status and running `ipconfig`.
- Attempted to access `\\fileserver\Legal_2025` from her workstation — received the same error.
- Verified the mapped drive letter pointed to the correct folder path.
- Tested access using a different account with similar permissions — worked successfully, indicating the issue was account-specific.
- Checked Priya’s Active Directory (AD) group memberships and found she was no longer part of the `Legal_Department` security group.

---

## Steps Taken to Resolve

1. **Confirmed Network and Folder Availability**

   - Pinged `fileserver` successfully.
   - Verified other shared folders were accessible from Priya’s account.

2. **Restored AD Group Membership**

   - Opened **Active Directory Users and Computers (ADUC)**.
   - Located Priya’s user account and confirmed missing `Legal_Department` membership.
   - Added her back to the `Legal_Department` security group.

3. **Applied Changes**

   - Instructed Priya to log off and log back in to refresh her Kerberos ticket.
   - Retested access — folder opened successfully without errors.

4. **Documented the Fix**
   - Updated IT change logs with the date, time, and change made.
   - Notified Priya and confirmed she could access and modify documents in the folder.

---

## Final Resolution

> _Priya’s account had been removed from the `Legal_Department` security group, which controlled access to the **Legal_2025** shared folder. Restoring her group membership resolved the issue immediately._

---

## Notes / Recommendations

- Review AD group change history to determine why the account was removed.
- Set up alerts for security group membership changes.
- Provide department leads with guidance on proper user account management to avoid accidental permission changes.

---

<p align="center">
  <a href="/tickets/ticket-007/README.md">⬅️ Previous (007)</a> • 
  <a href="/dashboard.md">🏠 Dashboard</a> • 
  <a href="/tickets/ticket-009/README.md">➡️ Next (009)</a>
</p>
