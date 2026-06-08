# Healthcare Payer Transformation Book Series - Microsite

A single-page marketing microsite for the 5-book Healthcare Payer Transformation series by Vikram Malhotra and Animesh Raj Jha.

## Features

- Responsive single-page design
- Smooth scroll animations
- Book showcase with Amazon buy links
- Business impact metrics
- Author profiles
- Mobile-friendly navigation

## Deploy to GitHub Pages

### Option 1: Quick Deploy (New Repository)

1. **Create a new GitHub repository**
   - Go to https://github.com/new
   - Name it something like `payer-books-microsite` or `healthcare-payer-books`
   - Make it **Public** (required for free GitHub Pages)
   - Don't initialize with README (we already have files)

2. **Push the microsite files**
   ```bash
   cd /Users/vik.malhotra/PayerBookWork/microsite
   git init
   git add .
   git commit -m "Initial microsite launch"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/payer-books-microsite.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Go to your repo's **Settings** > **Pages**
   - Under "Source", select **Deploy from a branch**
   - Choose **main** branch and **/ (root)** folder
   - Click **Save**

4. **Access your site**
   - Wait 1-2 minutes for deployment
   - Your site will be live at: `https://YOUR_USERNAME.github.io/payer-books-microsite/`

### Option 2: Custom Domain (Optional)

1. Purchase a domain (e.g., `payertransformation.com`)
2. Add a `CNAME` file to the repo with your domain
3. Configure DNS with your registrar:
   - Add CNAME record: `www` -> `YOUR_USERNAME.github.io`
   - Add A records for apex domain pointing to GitHub's IPs

## Local Development

To preview locally:

```bash
cd /Users/vik.malhotra/PayerBookWork/microsite
python3 -m http.server 8000
```

Then open http://localhost:8000 in your browser.

## File Structure

```
microsite/
├── index.html      # Main HTML file
├── styles.css      # All styles and animations
├── images/         # Book cover images
│   ├── book1-cover.jpg
│   ├── book2-cover.png
│   ├── book3-cover.jpg
│   ├── book4-cover.jpg
│   └── book5-cover.jpg
└── README.md       # This file
```

## Customization

- **Colors**: Edit CSS variables in `:root` section of `styles.css`
- **Content**: Edit text directly in `index.html`
- **Images**: Replace files in `images/` folder
- **Contact email**: Update the mailto link in the Contact section

## Books Included

1. **The Payer Business 101** - Healthcare insurance fundamentals
2. **The Payer Transformation Playbook** - Digital transformation strategy
3. **Call Quality Intelligence for Dummies** - AI-powered contact center analytics
4. **Metric Governance** - Building trusted healthcare analytics
5. **Next Best Action** - AI-driven member engagement
