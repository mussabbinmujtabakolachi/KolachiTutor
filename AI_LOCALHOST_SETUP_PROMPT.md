# One-Entry AI Setup Prompt

Copy everything below and send it to any AI coding agent as a single message.

```text
You are setting up and running a Next.js project locally.

Goal:
- Install all requirements for this project.
- Start the site on localhost.
- Confirm it is running.

Project path:
- Use the current working directory (this folder).

Do exactly these steps:
1) Detect OS (Windows/macOS/Linux).
2) Check whether Node.js and npm exist.
3) If missing, install Node.js LTS (20.x or newer) using the OS package manager:
   - Windows: winget install OpenJS.NodeJS.LTS
   - macOS: brew install node
   - Ubuntu/Debian: sudo apt-get update && sudo apt-get install -y nodejs npm
4) Verify versions:
   - node -v
   - npm -v
5) Install dependencies:
   - npm install
6) Run the development server:
   - npm run dev
7) Confirm local URL from terminal output (usually http://localhost:3000).
8) Verify HTTP response by requesting the URL and ensure it returns success.
9) Report back with:
   - Installed Node/npm versions
   - Final localhost URL
   - Whether the app is running successfully

If port 3000 is busy, run:
- npm run dev -- -p 3001
and report the updated URL.
```
