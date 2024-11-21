<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Secure the osTicket installation by removing or restricting access to sensitive directories.
- Configure essential system settings, including email integration for ticket notifications.
- Set up user roles, departments, and help topics to streamline ticket categorization.
- Optimize system performance with recommended server configurations.
- Enable monitoring and logging for troubleshooting and analytics.

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After installing osTicket, the first step in configuration is securing the installation to prevent unauthorized access and potential vulnerabilities. Begin by deleting the /setup directory from the installation path (e.g., C:\inetpub\wwwroot\osTicket) to remove access to the installer. Ensure sensitive files, like ost-config.php, have restricted permissions, allowing only the web server to read them. This step protects the core configuration details, such as database credentials. Additionally, enabling SSL on your web server is essential to encrypt all communication between users and the osTicket system.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, set up a user portal to allow customers or end-users to create tickets directly on the platform. Navigate to Admin Panel > Settings > User Portal, and customize the interface to reflect your organization's branding by adding a logo, adjusting the color scheme, and including a welcome message. Configure the fields users need to fill out when submitting tickets to gather all relevant information, such as contact details and the nature of their issue. Test the portal to ensure it is user-friendly and accessible. Providing a direct, easy-to-use portal improves the customer experience and reduces reliance on email-based ticketing.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Finally, customize the system to align with your organization's needs. Define departments, roles, and agents under Admin Panel > Agents to ensure an organized workflow. Set up help topics under Admin Panel > Manage > Help Topics to categorize tickets, making it easier for agents to prioritize and address issues. You can also create SLA plans to set response and resolution timeframes for different ticket types, ensuring timely customer support. These configurations not only enhance the efficiency of the support system but also improve user satisfaction.
</p>
<br />
