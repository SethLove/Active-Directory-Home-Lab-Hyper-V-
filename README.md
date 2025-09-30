# Active-Directory-Home-Lab-Hyper-V-
# Server Manager and Active Directory Configuration

This document outlines steps for configuring a server and integrating it into an Active Directory domain.

## Key Steps

1.  **Server Manager Installation:** Opened Server Manager and began a role-based installation. \
2.  **Active Directory Services Roles:** Installed the necessary features.
3.  **Promoted the server to a Domain Controller:**
    *   Added a new forest.
    *   Created a domain name.
    *   Created a password.
4.  **Group Policy Configuration:**
    *   Added employees into the group.
    *   Set Administrator as the group manager to login remotely via RDS.
    *   Added the "Allow log on through Remote Desktop Services" policy and added the employees' group to the policy.
    *   Modified Computer Configuration > Policies > Windows Settings > Security Settings > Local Policies > User Rights Assignment.

## Network Configuration

1.  Generated a Virtual Machine with Windows 11.
2.  Set DNS to the server's IP.
3.  Connected client VM to DC.
