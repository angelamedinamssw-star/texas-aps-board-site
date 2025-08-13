# APS Partners Board — Static Site Starter

This is a simple, responsive, accessible static website you can host for free on GitHub Pages or Netlify.

## Edit Content
- Open the `.html` files (e.g., `index.html`, `meetings.html`) in any text editor.
- Replace placeholder text (dates, names, links).
- Add PDFs to a `/docs` folder and update links on `meetings.html` and `policies.html`.

## Deploy to GitHub Pages
1. Create a free GitHub account (if needed).
2. Create a new repository (e.g., `aps-board-site`), **Public** is fine.
3. Upload all files from this folder.
4. Go to **Settings → Pages**: Under *Build and deployment*, pick **Deploy from a branch** and set **Branch: main / root**. Save.
5. Your site will publish to `https://<username>.github.io/aps-board-site/`.
6. **Custom domain**: In **Settings → Pages**, add your domain (e.g., `www.example.org`). Enable **Enforce HTTPS**.
7. **DNS setup** at your domain registrar:
   - For a subdomain like `www.example.org`: create a **CNAME** record pointing to `<username>.github.io`.
   - For the root (apex) like `example.org`: create **A** records to GitHub Pages IPs: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`. (Keep `www` as a CNAME to avoid issues.)

## Deploy to Netlify (drag-and-drop)
1. Go to https://app.netlify.com/ and sign up.
2. Click **Add new site → Deploy manually** and drag this folder into the browser.
3. After deploy, click **Domain settings → Add custom domain** and enter your domain (e.g., `www.example.org`).
4. **DNS options**:
   - Easiest: Use **Netlify DNS** and change nameservers at your registrar when prompted.
   - Or keep your registrar’s DNS:
     - Set `www` **CNAME** to your Netlify site subdomain (shown in Domain settings).
     - Set root `example.org` **A** records to Netlify load balancer IPs (currently `75.2.60.5` and `99.83.190.102`).

## Tips
- Changes go live when you re-upload or redeploy.
- Keep PDFs under 10–15 MB for fast loading.
- Turn on HTTPS (GitHub Pages or Netlify will issue free TLS certificates).