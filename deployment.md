# Overview
This document explains how the Joblinx website was created using WordPress. The process starts with building the site on a local computer and ends with making it live on a hosting platform. For easier understanding, the information is divided into sections and sub-files, covering each step of the process.

## Required Tools
- **Hosting Platform:** InfinityFree, a free hosting platform for this project. No payment is required for hosting here.
- **Local Development Environment:** XAMPP, a local server that provides Apache and MySQL databases to help the CMS run.
- **WP Vivid Backup:** WP Vivid, Plugin used to migrate website from local to hosting platform.
- **Version Control:** Git and GitHub, a repository storage platform to help in version control.
- **Project Management:** Trello, used for task management, project organization, team collaboration, and tracking workflows 				efficiently across various personal and professional projects.

## Local Development Process

### Step 1: XAMPP Installation
Download and install XAMPP from [apachefriends.org](https://www.apachefriends.org/).

### Step 2: Set Up WordPress
- Download the latest version of WordPress from [wordpress.org](https://wordpress.org/).
- Navigate to the `htdocs` directory of the XAMPP installation and create a folder named `a2.html`.
- Extract the WordPress files into the `a2.html`.
- Create a new database named `joblinx` using phpMyAdmin (accessible via `http://localhost/phpmyadmin`).
- Complete the WordPress installation by visiting `http://localhost/` and following the setup wizard.
- The setup wizard prompts you to connect the database and set up the admin logins, name of the site, and description.

### Step 3: Develop the Website
Use the admin WordPress dashboard to customize the theme.

### Step 4: Clone Repository
Clone the GitHub repository containing the project files into the `wp-content/themes` directory.

For more information about customizing the website, visit the `theme.md` file.

## Deployment on Live Server

### Finalize the Local WordPress Site to upload on deployment site.

### Step 1: Prepare and install wordpress on hosting site: 
- we created a domain site on infinity free and installed WordPress on that domain using Softaculous software installer provided by 	infinity cPanel.

### Step 2:Install WPvivid Plugin
- Install and activate the WPvivid Backup & Migration plugin on both the local site and the hosting site.

### Step 3:Create a Backup on the Local Site
- Go to WPvivid Backup in the local site’s dashboard.
- Click Backup Now to create a backup of the site.
- Once the backup is complete, download the backup file to your local machine by clicking the Download button.

### Step 4: Upload the Backup to the Hosting Site
- On the hosting site, go to WPvivid Backup > Upload.
- Upload the backup file you downloaded from the local site.

### Step 5: Restore the Backup on the Hosting Site
- Navigate to WPvivid Backup > Backups on the hosting site.
- Locate the uploaded backup file in the backup list.
- Click Restore to start the restoration process.
- Confirm the restoration when prompted.

### Step 6: Test the Site on the Hosting Environment
- After the restoration is complete, verify that the site is working correctly on the hosting environment.
- Update the site's URLs if necessary using the WPvivid tools or a plugin like Better Search Replace.

#### Test the Site:
- Access your website using the URL provided by InfinityFree to confirm it is live.  
- Conduct a detailed review to ensure all features and functionality are operating properly.
