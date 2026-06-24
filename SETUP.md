# Great Lakescape Website — Setup Guide

## What's in this folder

| File | What it does |
|------|-------------|
| `index.html` | Your website |
| `content.json` | All your text & settings (edit this to change anything) |
| `admin/` | Your built-in editor (access at greatlakescape.org/admin) |
| `netlify.toml` | Hosting configuration |

---

## Step 1 — Create a GitHub account (free)
1. Go to **github.com** and sign up (free)
2. Click **New repository**
3. Name it `greatlakescape-website`, set it to **Public**
4. Click **Create repository**
5. Upload all these files by clicking **uploading an existing file**

---

## Step 2 — Create a Netlify account (free)
1. Go to **netlify.com** and sign up with your GitHub account
2. Click **Add new site → Import an existing project**
3. Choose **GitHub** and select `greatlakescape-website`
4. Click **Deploy site**

Your site will go live at a random `.netlify.app` URL within 1 minute.

---

## Step 3 — Connect your domain (greatlakescape.org)
1. In Netlify, go to **Domain management → Add a domain**
2. Type `greatlakescape.org` and follow the prompts
3. Netlify will give you nameservers to point your domain to
4. Log in to wherever your domain is registered and update the nameservers

---

## Step 4 — Enable the site editor (admin panel)
This lets you edit text and photos at **greatlakescape.org/admin**

1. In Netlify, go to **Site configuration → Identity**
2. Click **Enable Identity**
3. Under **Registration**, choose **Invite only**
4. Go to **Services → Git Gateway** and click **Enable Git Gateway**
5. Back in Identity, click **Invite users** and enter your email
6. Check your email and accept the invite
7. Visit `greatlakescape.org/admin` — log in with your email

---

## Step 5 — Edit your site content

### Option A — Through the admin panel (easiest)
Go to `greatlakescape.org/admin` and use the visual editor to change any text, upload photos, etc.

### Option B — Edit content.json directly on GitHub
1. Go to your GitHub repo
2. Click on `content.json`
3. Click the pencil icon (Edit)
4. Make your changes
5. Click **Commit changes**

The site updates automatically within 30 seconds.

---

## Connecting Facebook
Your Facebook page URL is already set in `content.json`:
```
"facebook_url": "https://www.facebook.com/profile.php?id=61560578065406"
```
This is already connected and the Facebook feed embed will load on your live site.

## Connecting Google Business Profile
Update these two lines in `content.json`:
1. `"google_review_url"` — your Google review link (get it from your GBP dashboard → "Get more reviews")
2. `"google_maps_url"` — your Google Maps link

---

## Adding photos
To add a hero background photo:
1. Go to your admin panel
2. Click **Site Settings → Hero Section**
3. Click **Hero Background Photo** and upload a landscape photo
4. Save

To add a team/work photo to the About section:
1. Go to **Site Settings → About Section**
2. Click **Team / Work Photo** and upload
3. Save

---

## Updating your phone number
In `content.json`, change:
```json
"phone": "(248) 555-0000"
```
to your real number.

---

## Contact form
The contact form works automatically with Netlify Forms (free, up to 100 submissions/month).
Form submissions are emailed to you and visible at **Netlify → Forms**.
