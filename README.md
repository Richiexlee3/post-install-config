<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
After installing osTicket, you’ll create roles for admins and agents, deciding who can manage tickets. Then, you’ll set up departments (like IT or Support) to organize tickets and create SLAs to ensure quick responses. Finally, you’ll manage help topics and decide if users need to register before submitting tickets.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

Here are the **Top 5 Post-Install Configuration Objectives** for osTicket:

1. **Configure User Roles and Permissions**:  
   Set up roles like **Supreme Admin**, agents, and assign permissions for managing tickets and system settings.

2. **Organize Departments**:  
   Create departments (e.g., **SysAdmins**, **Networking**) to assign tickets and control visibility across different teams.

3. **Set Up Service Level Agreements (SLA)**:  
   Define response and resolution times based on ticket priority (e.g., **Sev-A**, **Sev-B**, **Sev-C**) to ensure timely support.

4. **Create and Manage Help Topics**:  
   Set up predefined help topics (e.g., **Business Critical Outage**, **Password Reset**) for users to select when creating tickets, improving ticket categorization.

5. **Configure Ticket Creation Settings**:  
   Decide whether to allow unregistered users to create tickets or require registration/login to ensure controlled ticket creation.

<h2>Configuration Steps</h2>
Here is a step-by-step guide for osTicket Post-Install Configuration to set up your help desk system effectively:

---

### **Step 1: Log In**
- **Admin/Analyst Login Page**: [http://localhost/osTicket/scp/login.php](http://localhost/osTicket/scp/login.php)  
  Use this URL to access the Admin or Agent Panel to configure and manage tickets.  
- **End Users URL**: [http://localhost/osTicket](http://localhost/osTicket)  
  This is where customers can create and check tickets.

---

### **Step 2: Acknowledge Panels**
- **Agent Panel**: Used by agents to respond to tickets and manage assigned tasks.  
- **Admin Panel**: For administrators to configure roles, permissions, users, and system settings.  

---

### **Step 3: Configure Roles (Group Permissions)**
1. Navigate to **Admin Panel -> Agents -> Roles**.
2. Create a role, e.g., **Supreme Admin**.
3. Assign permissions to define what agents with this role can do, like editing tickets or managing users.

---

### **Step 4: Configure Departments (Ticket Visibility)**
1. Go to **Admin Panel -> Agents -> Departments**.
2. Add departments to organize tickets:
   - Example: **SysAdmins**, **Networking**, **Help Desk**.
3. Assign tickets to specific departments for better management.

---

### **Step 5: Configure Teams**
1. Navigate to **Admin Panel -> Agents -> Teams**.
2. Create teams to group agents from different departments for specific tasks.
   - Example: **Online Banking Team**, which includes agents from SysAdmins and Help Desk.

---

### **Step 6: Allow or Restrict Ticket Creation**
1. Go to **Admin Panel -> Settings -> User Settings**.
2. **To allow anyone to create tickets**:
   - Uncheck **"Registration Required"**.
3. **To require user registration**:
   - Check **"Require registration and login to create tickets."**

---

### **Step 7: Configure Agents (Workers)**
1. Go to **Admin Panel -> Agents -> Add New**.
2. Add agent accounts:
   - Example:  
     - **Jane** (Department: SysAdmins).  
     - **John** (Department: Support).  

---

### **Step 8: Configure Users (Customers)**
1. Navigate to **Agent Panel -> Users -> Add New**.
2. Add customer accounts:
   - Example:
     - **Karen**.  
     - **Ken**.

---

### **Step 9: Configure SLA (Service Level Agreements)**
1. Go to **Admin Panel -> Manage -> SLA**.
2. Add SLA plans to define response times:
   - **Sev-A**: Grace Period = 1 hour, Schedule = 24/7.  
   - **Sev-B**: Grace Period = 4 hours, Schedule = 24/7.  
   - **Sev-C**: Grace Period = 8 hours, Schedule = Business Hours.

---

### **Step 10: Configure Help Topics**
1. Navigate to **Admin Panel -> Manage -> Help Topics**.
2. Add topics to help categorize tickets:
   - Examples:
     - **Business Critical Outage**.
     - **Personal Computer Issues**.
     - **Equipment Request**.
     - **Password Reset**.
     - **Other**.

---

By completing these steps, your osTicket system will be well-organized and ready for both agents and end users to manage and resolve tickets efficiently.
<p>
