# SRA SharePoint Login Helper

This repository hosts the **SRA SharePoint Login Helper**, a lightweight web page designed to assist users in accessing Shirley Ryan AbilityLab's SharePoint resources with the correct Microsoft 365 account.

[Visit the site on GitHub Pages](https://sra-mweber.github.io/sra-sp-login-helper/)

## 🔍 Purpose

Many users at SRA have multiple Microsoft 365 accounts (e.g., with Northwestern Medicine and SRA). This often leads to access issues when trying to open SharePoint links. This helper page ensures users are signed out of any existing Microsoft 365 session and then redirected to the appropriate SharePoint site.

## ⚙️ How It Works

Each button on the page performs the following steps using JavaScript:

1. **Logs the user out** of their current Microsoft 365 session via `https://login.microsoftonline.com/logout.srf`
2. **Waits briefly** (e.g., 3 seconds)
3. **Redirects** the user to the selected SRA SharePoint resource

This ensures users are prompted to log in with their SRA credentials.

## 🚀 Deployment via GitHub Pages

To deploy this site:

1. Clone or fork this repository
2. Ensure the main HTML file is named `index.html`
3. Go to **Settings > Pages** in your GitHub repository
4. Under **Source**, select the branch (e.g., `main`) and root folder (`/`)
5. GitHub will generate a public URL like:
