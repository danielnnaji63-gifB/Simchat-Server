# SimChat AI - Backend Server

## How to Deploy FREE on Render.com (Step by Step)

### STEP 1 - Get your Anthropic API Key
1. Go to https://console.anthropic.com
2. Sign up or log in
3. Click "API Keys" in the left menu
4. Click "Create Key"
5. Copy the key (starts with sk-ant-api03-...)

### STEP 2 - Put your files on GitHub
1. Go to https://github.com and create a free account
2. Click the "+" button → "New repository"
3. Name it "simchat-server"
4. Click "Create repository"
5. Upload ALL these files to it:
   - server.js
   - package.json
   - render.yaml
   - public/index.html

### STEP 3 - Deploy on Render.com (FREE)
1. Go to https://render.com and sign up free
2. Click "New" → "Web Service"
3. Connect your GitHub account
4. Select your "simchat-server" repository
5. Render will auto-detect the settings from render.yaml
6. Click "Advanced" → "Add Environment Variable"
   - Key:   ANTHROPIC_API_KEY
   - Value: paste your key from Step 1
7. Click "Create Web Service"
8. Wait 2-3 minutes for it to deploy
9. Render gives you a FREE URL like: https://simchat-server.onrender.com

### STEP 4 - Open your app
- Visit your Render URL in any browser
- SimChat AI now works fully — chat, voice, history, clock, calculator
- Share the URL with anyone!

## Running Locally (on your own computer)
1. Install Node.js from https://nodejs.org
2. Open terminal in this folder
3. Run: npm install
4. Create a .env file and add: ANTHROPIC_API_KEY=your-key-here
5. Run: npm start
6. Open http://localhost:3000 in your browser

## Files Explained
- server.js        → The backend server (talks to Anthropic API)
- package.json     → Lists the packages the server needs
- render.yaml      → Tells Render.com how to run your server
- public/index.html → Your SimChat app (the frontend)
- .env.example     → Template for your API key file
