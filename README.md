# m365-entra-lab
Microsoft 365 and Entra ID IT Admin Lab
# Microsoft 365 & Entra ID — IT Admin Lab

Hands-on lab simulating real-world IT helpdesk workflows using 
Microsoft 365 and Microsoft Entra ID.

## Tenant Details
- Organisation: Mock Agency
- Domain: mockagency.onmicrosoft.com
- Platform: Microsoft 365 Business Standard

---

## Task 1 — Tenant Setup
- Created Microsoft 365 Business Standard trial tenant
- Configured Global Administrator account

---

## Task 2 — User Provisioning
- Created user: John Smith (jsmith@mockagency.onmicrosoft.com)
- Created user: Sarah Jones (sjones@mockagency.onmicrosoft.com)
- Assigned Microsoft 365 Business Standard license to both users
- Set password change required on first login

<img width="441" height="461" alt="addition of John Smith" src="https://github.com/user-attachments/assets/52e6dac5-3cdc-463d-aeb5-d0ce3e912257" />

<img width="473" height="493" alt="Sarah Jones onboarding" src="https://github.com/user-attachments/assets/b259f490-367d-423b-8949-06cdff55c65c" />


---

## Task 3 — Security Group
- Created IT-Staff security group in Entra ID
- Added John Smith and Sarah Jones as members

<img width="476" height="484" alt="Adding john and sarah to security group" src="https://github.com/user-attachments/assets/077b6106-a823-487f-99a8-470c7e986a96" />

---

## Task 4 — MFA Configuration
- Enabled per-user MFA for John Smith and Sarah Jones
- Configured via Entra ID → Users → Per-user MFA

<img width="480" height="564" alt="per user mfa" src="https://github.com/user-attachments/assets/ee0a0619-2ca8-4642-bdb6-e1109c7428f8" />

---

## Task 5 — Self-Service Password Reset (SSPR)
- Enabled SSPR in Entra ID scoped to IT-Staff group
- Users can reset passwords at aka.ms/sspr

<img width="480" height="564" alt="Default password reset " src="https://github.com/user-attachments/assets/16a75cf2-efcb-4dc1-8faf-c287e2ad6e31" />

<img width="960" height="1128" alt="Screenshot 2026-03-22 212506" src="https://github.com/user-attachments/assets/32ec9939-c1a0-4371-8c3b-330c6df64367" />

---

## Task 6 — Offboarding (Sarah Jones)
Full leaver workflow completed:
1. Disabled account in Entra ID
2. Revoked all active cloud sessions
3. Removed Microsoft 365 license
4. Removed from IT-Staff security group
5. Deleted user account
<img width="480" height="564" alt="offboarding sarahjones 1" src="https://github.com/user-attachments/assets/a0b1a4da-1ba3-4f37-adf2-bab1d6f44bd1" />

<img width="960" height="1128" alt="Screenshot 2026-03-22 212846" src="https://github.com/user-attachments/assets/3dea2acf-623b-4fd5-b5e5-1e6cc8e33034" />

<img width="480" height="564" alt="offboarding sarahjones2" src="https://github.com/user-attachments/assets/416acc98-c462-49ea-af1f-e08a3369b1d1" />

<img width="480" height="564" alt="Sarah Jones offboarding two" src="https://github.com/user-attachments/assets/3376679b-68c8-4cae-8054-8592fdcada9e" />

---

## Tools Used
- Microsoft 365 Admin Center (admin.microsoft.com)
- Microsoft Entra Admin Center (entra.microsoft.com)
- PowerShell (AD module)
