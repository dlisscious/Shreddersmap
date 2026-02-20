# Metal Shredders Map - Vercel Deployment

## Quick Deployment Steps

### Option 1: Deploy via Vercel CLI (Recommended)

1. **Install Vercel CLI** (if you haven't already):
   ```bash
   npm install -g vercel
   ```

2. **Navigate to this directory**:
   ```bash
   cd deploy_package
   ```

3. **Deploy**:
   ```bash
   vercel
   ```
   
   - First time: Login with your Vercel account
   - Follow the prompts (press Enter to accept defaults)
   - Your site will be live in seconds!

4. **Deploy to production**:
   ```bash
   vercel --prod
   ```

### Option 2: Deploy via Vercel Dashboard (No CLI needed)

1. Go to [vercel.com](https://vercel.com) and sign up/login
2. Click "Add New Project"
3. Choose "Import Git Repository" OR "Deploy from Template"
4. If using Git:
   - Push this folder to a GitHub/GitLab/Bitbucket repo
   - Import that repo in Vercel
5. If deploying directly:
   - Drag and drop this entire `deploy_package` folder into Vercel
6. Click "Deploy"

### Option 3: Deploy via GitHub

1. Create a new GitHub repository
2. Push this `deploy_package` folder contents to the repo:
   ```bash
   git init
   git add .
   git commit -m "Initial commit - Metal Shredders Map"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
   git push -u origin main
   ```
3. Go to [vercel.com](https://vercel.com)
4. Click "Import Project" → "Import Git Repository"
5. Select your GitHub repo
6. Click "Deploy"

## What's Included

- `index.html` - The interactive map with all features:
  - 278 scrap metal shredder locations (red dots)
  - 18 independent market shredders (green dots) - 75 mile radius, <4 locations, excluding DJJ/Nucor
  - 68 electric arc furnace steel mills (blue dots)
  - Search and filter functionality
  - Interactive legend
  - OpenStreetMap base layer

- `vercel.json` - Vercel configuration (handles routing)

## After Deployment

Your map will be available at:
- Preview: `https://your-project-name-random.vercel.app`
- Production: `https://your-project-name.vercel.app`

You can also add a custom domain in the Vercel dashboard.

## Updating the Map

To update your deployed map:
1. Replace `index.html` with the new version
2. Run `vercel --prod` (CLI) or push to Git (if using Git integration)

## Support

- Vercel Docs: https://vercel.com/docs
- Vercel CLI: https://vercel.com/docs/cli
