# DonationReceipt

Simple static donation receipt app for Masjid Ibrahim. The app runs fully in the browser and sends receipts using EmailJS.

## Run locally

Because this is a static site, you can use any static server:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Deploy to Vercel

This repo is Vercel-ready as a static site.

1. Import the GitHub repository into Vercel.
2. Leave build settings empty:
	- Build Command: none
	- Output Directory: none
3. Deploy.

`vercel.json` already rewrites all routes to `index.html` so direct links continue to work.

## First-time app setup

After deployment, open the app and click EmailJS Settings to add:

- Public Key
- Service ID
- Template ID

Those keys are stored in browser local storage on that device.