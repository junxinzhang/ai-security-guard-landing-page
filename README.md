# AI Security Guard - Landing Page

> Enterprise AI Security Protection Platform - Build security for your AI applications.

![Page Preview](assets/screenshot.jpg)

## Project Overview

This is the official landing page for AI Security Guard, showcasing product features, technical architecture, and quick start guide.

### Core Features

- Modern responsive design
- Lightweight static website (no backend required)
- Chinese and English bilingual support
- Perfect mobile support
- Accessibility compliant
- SEO friendly (Schema.org structured data)
- Image carousel showcase (16 screenshots)
- Scroll animations (AOS)
- PWA support

## Technology Stack

- **Frontend**: Pure HTML5 + CSS3 + JavaScript
- **CSS Framework**: Tailwind CSS (CDN)
- **Icon Library**: Remix Icon
- **Animation Library**: AOS (Animate On Scroll)
- **Deployment**: GitHub Pages

## Project Structure

```
ai-security-guard-landing-page/
├── index.html              # Chinese homepage
├── en/
│   └── index.html          # English homepage
├── css/
│   └── style.css           # Global styles
├── js/
│   └── main.js             # Interaction scripts
├── assets/                 # Resource files
│   ├── favicon.png         # Website icon
│   ├── icon.png            # PWA icon
│   ├── logo.png            # Logo
│   ├── screenshot.jpg      # Screenshot 1
│   ├── screenshot01.jpg    # Screenshot 2
│   ├── screenshot02.jpg    # Screenshot 3
│   ├── ...                 # Screenshots 4-15
│   ├── screenshot15.jpg    # Screenshot 16
│   └── JustJason_wechat-qrcode.jpg  # WeChat QR code
├── .github/
│   └── workflows/
│       └── static.yml      # GitHub Actions workflow
├── CNAME                   # Custom domain config
├── manifest.json           # PWA configuration
├── robots.txt              # Crawler configuration
├── sitemap.xml             # Sitemap
└── README.md               # Project description
```

## Quick Start

### Local Preview

1. Clone the project
```bash
git clone https://github.com/junxinzhang/ai-security-guard-landing-page.git
cd ai-security-guard-landing-page
```

2. Start a local server (choose one)

**Using Python**:
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

**Using Node.js**:
```bash
npx http-server -p 8000
```

**Using PHP**:
```bash
php -S localhost:8000
```

3. Open `http://localhost:8000` in your browser

### Deploy to GitHub Pages

#### Method 1: Enable via Repository Settings (Recommended)

1. Push code to GitHub repository
```bash
git add .
git commit -m "Update: Landing page content"
git push origin main
```

2. In the GitHub repository:
   - Go to **Settings** → **Pages**
   - Set **Source** to `GitHub Actions`
   - Workflows will trigger deployment automatically

3. After deployment, visit:
   ```
   https://YOUR_USERNAME.github.io/ai-security-guard-landing-page/
   ```

#### Method 2: Manual Workflow Trigger

In the GitHub repository's **Actions** tab, select the corresponding workflow and click **Run workflow** to trigger manually.

## Customization

### Modify Color Theme

Edit CSS variables in `css/style.css`:

```css
:root {
  --color-blue-500: #3b82f6;    /* Primary color */
  --color-purple-500: #8b5cf6;  /* Accent color */
  /* ... */
}
```

### Modify Content

- Edit `index.html` to modify Chinese content
- Edit `en/index.html` to modify English content

### Replace Screenshots

Place new screenshot files in the `assets/` directory:
- `screenshot.jpg` (Carousel image 1)
- `screenshot01.jpg` to `screenshot15.jpg` (Carousel images 2-16)

Recommended size: 900x600px (JPG format)

## Features

### Image Carousel

- Auto-play (5 second interval)
- 16 product screenshots
- Left/right arrow buttons
- Bottom indicators
- Keyboard arrow navigation
- Touch swipe support
- Pause on hover

### Responsive Design

- Mobile hamburger menu
- Adaptive layout
- Touch-friendly interactions

### PWA Support

- Installable to desktop
- Offline access support
- Native app experience

## Multiple Deployment Options

### Nginx

```nginx
server {
    listen 80;
    server_name aisecguard.junxinzhang.com;
    root /path/to/ai-security-guard-landing-page;
    index index.html;

    location / {
        try_files $uri $uri/ =404;
    }
}
```

### AWS S3

1. Create S3 bucket
2. Upload all files
3. Configure static website hosting
4. Configure CloudFront (optional)

## Analytics Integration

The landing page includes placeholder comments for analytics integration. To enable analytics:

1. **Google Analytics**: Replace `YOUR_GA_ID` with your Google Analytics ID
2. **Baidu Analytics**: Replace `YOUR_BAIDU_KEY` with your Baidu Analytics key
3. **Umami Analytics**: Replace `YOUR_UMAMI_ID` with your Umami website ID

Uncomment the corresponding script blocks in both `index.html` and `en/index.html`.

## Reference Links

- **Product Website**: https://aisecguard.junxinzhang.com
- **Project Repository**: https://github.com/junxinzhang/ai-security-guard-landing-page

## Author

**Jason Zhang**

- Email: jason2023zhang@gmail.com
- Twitter/X: [@Jasonz9788](https://x.com/Jasonz9788)
- Blog: [https://junxinzhang.com](https://junxinzhang.com)
- WeChat: winnielove2020

## License

MIT

---

If this project helps you, please give it a Star!
