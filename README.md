# Happy Birthday Page 🎉

An immersive scroll-based birthday message page with beautiful background images, scroll-reveal animations, and a line-by-line message display.

## Features
- 🎨 **Scroll-based storytelling** - Multiple sections that reveal as you scroll
- 🖼️ **Background image transitions** - Your photos appear as backgrounds during scroll
- 📜 **Line-by-line message reveal** - Only 3 lines visible at a time, new lines appear as you scroll
- 🎊 **Falling confetti** effect
- 📱 **Fully responsive** design for mobile and desktop
- ✨ **Smooth animations** and transitions

## Setup Instructions

### 1. Add Your Images

**IMPORTANT:** Save your two images in the `images/` folder with these exact names:
- `image1.jpg` - First couple image (will appear during message section)
- `image2.jpg` - Second couple image (will appear during personal message section)

The images should be in JPG format. If they're PNG, either convert them or update the file references in `index.html` (lines 68-72).

### 2. Customize the Message

Edit the message lines at lines 373-382 in `index.html`:
```html
<div class="message-line">Your custom line 1</div>
<div class="message-line highlight">Your custom line 2 (highlighted)</div>
...
```

Add your personal message at lines 393-395:
```html
Dear [Name],<br><br>
[Your heartfelt message here]
```

### 3. Test Locally

Run a local server:
```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000` in your browser and **scroll down** to see the effects!

## Deploying to GitHub Pages

1. **Push to GitHub:**
   ```bash
   git add .
   git commit -m "Add birthday message page with scroll effects"
   git push origin main
   ```

2. **Enable GitHub Pages:**
   - Go to your repository on GitHub
   - Click on **Settings**
   - Scroll down to **Pages** section (left sidebar)
   - Under **Source**, select `main` branch
   - Select `/` (root) as the folder
   - Click **Save**

3. **Access your site:**
   - Your site will be available at: `https://[your-username].github.io/happy-birthday/`
   - It may take a few minutes for the page to be live

## How It Works

The page has 4 scroll sections:
1. **Intro** - Happy Birthday title with scroll hint
2. **Message Reveal** - Scrollable message with 3 lines visible at a time (image1 background)
3. **Personal Note** - Your custom personal message (image2 background)
4. **Final Wishes** - Closing celebration

Enjoy celebrating! 🎂🎉
