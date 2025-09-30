# Active Directory Home Lab (Hyper-V)  
## Server Manager & Active Directory Configuration  

This project demonstrates the process of configuring a Windows Server, promoting it to a Domain Controller, and integrating a client machine into an Active Directory environment using Hyper-V.  

---

## 🚀 Key Steps  

1. **Server Manager Installation**  
   - Opened **Server Manager** and performed a role-based installation.  
   ![image alt](https://github.com/SethLove/Active-Directory-Home-Lab-Hyper-V-/blob/3525ffdb24cce117570641665badcae74c0c1dc1/Screenshot%202025-09-29%20191749.png)  

2. **Static IP Assignment**  
   - Configured a static IP address for the server.  
   ![image alt](https://github.com/SethLove/Active-Directory-Home-Lab-Hyper-V-/blob/3525ffdb24cce117570641665badcae74c0c1dc1/Screenshot%202025-09-29%20192655.png)  

3. **Active Directory Domain Services (AD DS) Installation**  
   - Installed Active Directory Domain Services and supporting features.  
   ![image alt](https://github.com/SethLove/Active-Directory-Home-Lab-Hyper-V-/blob/3525ffdb24cce117570641665badcae74c0c1dc1/Screenshot%202025-09-29%20191901.png)  

4. **Promoting the Server to a Domain Controller**  
   - Created a **new forest** and defined a domain name.  
   ![image alt](https://github.com/SethLove/Active-Directory-Home-Lab-Hyper-V-/blob/3525ffdb24cce117570641665badcae74c0c1dc1/Screenshot%202025-09-29%20193307.png)  
   - Set up a **Directory Services Restore Mode (DSRM) password**.  
   ![image alt](https://github.com/SethLove/Active-Directory-Home-Lab-Hyper-V-/blob/3525ffdb24cce117570641665badcae74c0c1dc1/Screenshot%202025-09-29%20193343.png)  

5. **Group Policy Configuration**  
   - Created an **Employees** security group and provisioned user accounts.  
   ![image alt](https://github.com/SethLove/Active-Directory-Home-Lab-Hyper-V-/blob/3525ffdb24cce117570641665badcae74c0c1dc1/Screenshot%202025-09-29%20194724.png)  
   - Assigned the **Administrator** as group manager with Remote Desktop Services (RDS) permissions.  
   ![image alt](https://github.com/SethLove/Active-Directory-Home-Lab-Hyper-V-/blob/3525ffdb24cce117570641665badcae74c0c1dc1/Screenshot%202025-09-29%20194730.png)  
   - Configured Group Policy:  
     - Navigated to: `Computer Configuration > Policies > Windows Settings > Security Settings > Local Policies > User Rights Assignment`  
     - Enabled **"Allow log on through Remote Desktop Services"** for the Employees group.  
     ![image alt](https://github.com/SethLove/Active-Directory-Home-Lab-Hyper-V-/blob/3525ffdb24cce117570641665badcae74c0c1dc1/Screenshot%202025-09-29%20195636.png)  

---

## 🌐 Network Configuration  

1. Created a **Windows 11 client virtual machine**.  
2. Configured the client’s **DNS** to point to the server’s IP.  
   ![image alt](https://github.com/SethLove/Active-Directory-Home-Lab-Hyper-V-/blob/3525ffdb24cce117570641665badcae74c0c1dc1/Screenshot%202025-09-29%20200820.png)  
3. Successfully **joined the client VM to the domain**.  
   ![image alt](https://github.com/SethLove/Active-Directory-Home-Lab-Hyper-V-/blob/3525ffdb24cce117570641665badcae74c0c1dc1/Screenshot%202025-09-29%20201319.png)  
4. Verified **remote login to the domain** from the client machine.  
   ![image alt](https://github.com/SethLove/Active-Directory-Home-Lab-Hyper-V-/blob/3525ffdb24cce117570641665badcae74c0c1dc1/Screenshot%202025-09-29%20201544.png)  
   ![image alt](https://github.com/SethLove/Active-Directory-Home-Lab-Hyper-V-/blob/3525ffdb24cce117570641665badcae74c0c1dc1/Screenshot%202025-09-29%20201757.png)  

---

✅ **Setup Complete!**  
Your Hyper-V Active Directory lab environment is now fully configured and ready for use.  
