# Pat Gray Bingo

Interactive bingo tracker for the Pat Gray Show. Upload a new card photo each week and AI auto-parses the squares.

## Deploy to Railway (5 minutes)

### 1. Push to GitHub
```bash
git init
git add .
git commit -m "Pat Gray Bingo"
# Create a new repo on github.com, then:
git remote add origin https://github.com/YOUR_USERNAME/patgray-bingo.git
git push -u origin main
```

### 2. Deploy on Railway
1. Go to [railway.app](https://railway.app) and sign in with GitHub
2. Click **New Project → Deploy from GitHub repo**
3. Select your `patgray-bingo` repo
4. Once deployed, go to **Variables** and add:
   - `ANTHROPIC_API_KEY` = your key from [console.anthropic.com](https://console.anthropic.com)
5. Go to **Settings → Networking → Generate Domain** to get your public URL

That's it — share the URL with listeners!

## Update the card each week
1. Open your app URL
2. Click **Update card (new week)**
3. Upload a photo of the new bingo sheet
4. AI parses all 25 squares automatically

## Run locally
```bash
npm install
ANTHROPIC_API_KEY=your_key_here node server.js
# Open http://localhost:3000
```
