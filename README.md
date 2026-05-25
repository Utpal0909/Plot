**Enterprise Dashboard SaaS Portal**
A modern, enterprise-grade dashboard portal built using HTML, CSS, and JavaScript, integrating Microsoft Azure (Entra ID) authentication, role-based access control, and an enhanced user experience similar to professional BI tools such as Power BI and Tableau.

** Overview**
This project is a fully functional BI portal UI designed to simulate a corporate dashboard system with:

Secure Microsoft login (Azure AD)
Role-based dashboard visibility
Favorites (starred dashboards)
Full-screen dashboard mode
Dark mode support
Smooth UI animations

👉 Designed as a real-world prototype for internal BI platforms

🔐 Features
✅ Authentication

Microsoft Login (Azure / Entra ID integration)
Only @l-acoustics.com users allowed
Session stored using localStorage
Secure logout functionality


🧠 Role-Based Access Control (RBAC)

































RoleAccessMasterAll departmentsFinanceFinance dashboards onlySalesSales dashboards onlyProcurementProcurement dashboardsITIT dashboardsOperationsOperations dashboards
👉 Roles are mapped dynamically based on user email.

⭐ Favorites System

Star dashboards to save as favorites
Favorites persist using localStorage
Dedicated Favorites section in sidebar
Instant access to most-used dashboards


📂 Dashboard Navigation

Expandable department sections (accordion UI)
4 dashboards per department
Smooth animations and transitions


🎨 UI / UX Enhancements

Dark mode toggle (persistent)
Professional layout and spacing
Hover interactions and animations
Responsive structure


🖥 Fullscreen Experience

One-click fullscreen mode
Sidebar auto-hide
Floating control buttons (exit, refresh)
Optimized viewing for embedded dashboards


⚡ Performance Features

Single iframe reused for all dashboards
Loading spinner while switching dashboards
Fast client-side interactions


🛠 Tech Stack

Frontend: HTML5, CSS3, JavaScript
Authentication: Microsoft Azure Entra ID (MSAL.js)
Hosting: GitHub Pages / Netlify / Azure Static Web Apps
Data Source: Power BI Embedded


📦 Project Structure
index.html       → Main application file
README.md        → Documentation


⚙️ Setup Instructions
1️⃣ Clone Repository
Shellgit clone https://github.com/your-username/your-repo.gitShow more lines

2️⃣ Configure Azure Authentication

Go to Azure Portal → App Registrations
Create a new App
Add:

Redirect URI (your website URL)
Enable ID tokens


Copy:

Client ID
Tenant ID



👉 Add them in your script:
JavaScriptconst msalConfig = {  auth: {    clientId: "YOUR_CLIENT_ID",    authority: "https://login.microsoftonline.com/YOUR_TENANT_ID",    redirectUri: "YOUR_WEBSITE_URL"  }};Show more lines

3️⃣ Run the App
Simply open:
index.html

or deploy using:

✅ GitHub Pages
✅ Netlify
✅ Azure Static Web Apps


🔒 Security Notes
⚠️ This project implements:

Client-side authentication (demo level)
Role-based visibility (frontend-controlled)

👉 For production:

Use Azure App Roles
Enforce backend validation
Secure Power BI access via Microsoft permissions


📈 Future Improvements

✅ Azure-driven roles (no hardcoding)
✅ Backend authentication (Node.js / APIs)
✅ KPI widgets and analytics layer
✅ Dashboard usage tracking
✅ Admin panel for role management


💼 Use Cases

Internal BI portal prototype
Corporate dashboard platform demo
Portfolio / resume project
Training project (frontend + auth systems)


👤 Author
Utpal UTKARSH
Purchasing Analyst (Trainee)
