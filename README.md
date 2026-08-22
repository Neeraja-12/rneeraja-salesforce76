# Salesforce Integration App

A full-stack Web Application for integrating custom CRM workflows with Salesforce using OAuth2 authentication and REST APIs.

## Features

- **Salesforce OAuth2 Authentication:** Secure connection using Consumer Key, Consumer Secret, and Callback URIs.
- **Full CRUD Operations:** Manage Salesforce standard objects (Accounts, Contacts, Opportunities, Leads, Cases) directly through the custom portal.
- **Production Deployment:** Deployed on Vercel with automated routing for full-stack Node.js Express backend and React frontend.
- **Environment Security:** Sensitive credentials managed safely via environment variables in development and production environments.

## Tech Stack

- **Frontend:** React.js, HTML5, CSS3, JavaScript (ES6+)
- **Backend:** Node.js, Express.js, JSforce / Axios
- **API:** Salesforce REST API (OAuth 2.0 Web Server Flow)
- **Deployment:** Vercel

## Project Structure

```text
RNeeraja-SalesForce/
├── backend/          # Express server and Salesforce OAuth/API routes
├── frontend/         # React client applications and public assets
├── vercel.json       # Vercel deployment routes and build configurations
├── .gitignore        # Ignored files (node_modules, .env, build, etc.)
└── README.md         # Project documentation
Getting Started
Prerequisites
Node.js (v18 or higher)

npm or yarn

Salesforce Developer Account with a Connected App created

Local Setup
Clone the repository:

Bash
git clone [https://github.com/Neeraja-12/RNeeraja-SalesForce.git](https://github.com/Neeraja-12/RNeeraja-SalesForce.git)
cd RNeeraja-SalesForce
Install backend dependencies:

Bash
cd backend
npm install
Install frontend dependencies:

Bash
cd ../frontend
npm install
Configure Environment Variables:
Create a .env file inside the backend/ directory:

Code snippet
PORT=5000
CLIENT_ID=your_salesforce_consumer_key
CLIENT_SECRET=your_salesforce_consumer_secret
REDIRECT_URI=http://localhost:5000/auth/callback
FRONTEND_URL=http://localhost:3000
Run the Application locally:

Backend:

Bash
cd backend
npm start
Frontend:

Bash
cd frontend
npm start
Production Deployment (Vercel)
Set Environment Variables in Vercel Dashboard > Settings > Environment Variables:

CLIENT_ID: Your Salesforce Consumer Key

CLIENT_SECRET: Your Salesforce Consumer Secret

REDIRECT_URI: https://rneeraja-salesforce76.vercel.app/auth/callback

FRONTEND_URL: https://rneeraja-salesforce76.vercel.app

Deploy using Vercel CLI:

PowerShell
vercel --prod
Live Demo
Application URL: https://rneeraja-salesforce76.vercel.app

Callback URL: https://rneeraja-salesforce76.vercel.app/auth/callback


---

### How to update it on GitHub

1. Replace the text inside your **`README.md`** file with the code block above and save it.
2. Run these commands in your PowerShell terminal:

```powershell
git add README.md
git commit -m "Update README with full-stack details and Vercel deployment setup"
git push
