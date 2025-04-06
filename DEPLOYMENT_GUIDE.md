# Sandwich Attack Simulator - Deployment Guide

This guide will help you deploy the improved Sandwich Attack Simulator to GitHub Pages so your Substack audience can access it.

## Prerequisites

- A GitHub account (free)
- Basic knowledge of using GitHub (or just follow these step-by-step instructions)

## Step 1: Create a New GitHub Repository

1. Go to [GitHub](https://github.com/) and sign in to your account
2. Click on the "+" icon in the top-right corner and select "New repository"
3. Name your repository (e.g., "sandwich-attack-simulator")
4. Make sure it's set to "Public"
5. Click "Create repository"

## Step 2: Upload the Files

### Option 1: Using GitHub Web Interface (Easiest)

1. In your new repository, click on the "Add file" button and select "Upload files"
2. Drag and drop all the files from the extracted zip folder into the upload area
3. Add a commit message like "Initial upload of Improved Sandwich Attack Simulator"
4. Click "Commit changes"

### Option 2: Using Git Command Line (For Advanced Users)

If you're comfortable with Git:

```bash
git clone https://github.com/YOUR-USERNAME/sandwich-attack-simulator.git
cd sandwich-attack-simulator
# Copy all files from the extracted zip folder to this directory
git add .
git commit -m "Initial upload of Improved Sandwich Attack Simulator"
git push origin main
```

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on "Settings" (tab near the top)
3. Scroll down to the "GitHub Pages" section
4. Under "Source", select "main" branch
5. Click "Save"
6. Wait a few minutes for GitHub to deploy your site

## Step 4: Access Your Deployed Simulator

1. After GitHub Pages is enabled, you'll see a message saying "Your site is published at https://YOUR-USERNAME.github.io/sandwich-attack-simulator/"
2. This is the URL you can share with your Substack audience

## Step 5: Share with Your Audience

1. In your Substack article, include the link to your GitHub Pages site
2. You might want to add some context like:
   
   "I've created an interactive Sandwich Attack Simulator to help you understand how these attacks work in DeFi. Try it out here: [Sandwich Attack Simulator](https://YOUR-USERNAME.github.io/sandwich-attack-simulator/)"

## Improvements in This Version

This improved version of the Sandwich Attack Simulator includes the following fixes:

1. **Corrected Price Impact Calculation**: The formula now correctly calculates price impact as `(expectedOutput - actualOutput) / expectedOutput * 100`

2. **Improved X-Axis Labeling**: The visualization now clearly labels transaction steps as:
   - 0% (Initial)
   - 25% (Front-Run)
   - 50% (Victim Trade)
   - 75% (Back-Run)
   - 100% (Final)

3. **Clarified Natural Slippage Visualization**: Now correctly shows how attacks amplify slippage rather than decrease it

4. **Enhanced Profit Calculation Transparency**: Clearly shows how profit is calculated:
   `Profit = Back-run ETH (4.00) - Front-run ETH (4.00) - Fees (0.0119 ETH) = -0.0119 ETH`

## Troubleshooting

- If your site doesn't appear after a few minutes, check the "Actions" tab in your GitHub repository to see if there are any deployment errors
- Make sure all files were uploaded correctly, especially the index.html file which should be in the root directory
- If you encounter any issues, feel free to reach out for assistance

## Updating the Simulator in the Future

If you want to make updates to the simulator:

1. Make your changes locally
2. Upload the new files to GitHub using the same process as above
3. GitHub Pages will automatically update your site with the new changes

---

That's it! Your improved Sandwich Attack Simulator is now deployed and accessible to your audience.
