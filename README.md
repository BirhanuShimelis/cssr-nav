# CSSR-Nav Project Page

Academic project page for **CSSR-Nav: Culturally Sensitive Social Robot Navigation Using Open-Source Vision-Language Models and Empirical Cultural Knowledge**.

## Local Preview

Open `index.html` in a browser, or use a local server:

```bash
cd cssr-nav.github.io
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Adding Videos

Place video files in the `assets/` folder:

- `assets/teaser.mp4` - Main teaser video
- `assets/personal_space.mp4` - Personal space demo
- `assets/group_avoidance.mp4` - Group avoidance demo
- `assets/greeting.mp4` - Greeting behavior demo

Then uncomment the corresponding `<video>` tags in `index.html` (search for "Uncomment when video is ready").

## Adding the Paper PDF

Place the paper PDF as `assets/paper.pdf`.

## Deploy to GitHub Pages

### Step 1: Create a GitHub Repository

Go to [github.com/new](https://github.com/new) and create a repository named:

- **Option A (organization page):** `cssr4africa.github.io` — the site will be at `https://cssr4africa.github.io`
- **Option B (project page):** `cssr-nav` — the site will be at `https://cssr4africa.github.io/cssr-nav`

### Step 2: Push the code

```bash
cd cssr-nav.github.io
git init
git add .
git commit -m "Initial commit: CSSR-Nav project page"
git branch -M main
git remote add origin git@github.com:cssr4africa/cssr-nav.github.io.git
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** > **Pages** (in the left sidebar)
3. Under **Source**, select **Deploy from a branch**
4. Select **main** branch and **/ (root)** folder
5. Click **Save**

The site will be live at `https://cssr4africa.github.io` (or `https://cssr4africa.github.io/cssr-nav/` for a project page) within a few minutes.

### Custom Domain (Optional)

To use a custom domain like `cssr-nav.org`:

1. In repository Settings > Pages, enter your custom domain
2. Add a `CNAME` file to the repo root containing your domain name
3. Configure DNS with your domain provider:
   - For apex domain: A records pointing to GitHub's IPs
   - For subdomain: CNAME record pointing to `cssr4africa.github.io`

## Project Structure

```
cssr-nav.github.io/
├── index.html                  # Main page
├── assets/                     # Videos and paper PDF
├── static/
│   ├── css/
│   │   ├── index.css           # Custom styles
│   │   ├── bulma.min.css       # Bulma CSS framework
│   │   ├── bulma-carousel.min.css
│   │   ├── bulma-slider.min.css
│   │   └── fontawesome.all.min.css
│   ├── js/
│   │   ├── index.js            # Custom scripts
│   │   ├── bulma-carousel.min.js
│   │   ├── bulma-slider.min.js
│   │   └── fontawesome.all.min.js
│   └── images/                 # Diagrams and figures
├── .gitignore
└── README.md
```

## Credits

Website template adapted from [Nerfies](https://nerfies.github.io), licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).
