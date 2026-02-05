# 💝 Valentine's Day Interactive Proposal

A fun, interactive Valentine's Day proposal webpage with playful animations and customizable options!

## ✨ Features

- 🎯 Interactive "Yes" and "No" buttons with fun mechanics
- 💖 Floating hearts animation on acceptance
- 🎵 Celebration music and sound effects
- 📱 Fully responsive design
- 🎨 Easy customization - no coding required!

## 🚀 Quick Start

1. **Download the files**
   - Click the green "Code" button above
   - Select "Download ZIP"
   - Extract the files to a folder

2. **Customize your page**
   - Open `valentine.html` in any text editor (Notepad, VS Code, etc.)
   - Find the `USER CONFIGURATION` section (around line 170)
   - Change the values as described below

3. **Test it out**
   - Simply double-click `valentine.html` to open in your browser
   - See your changes in action!

4. **Share with your Valentine**
   - Upload to GitHub Pages, Netlify, or any web hosting
   - Or send them the HTML file directly

## 🎨 How to Customize

Open `valentine.html` and find this section in the code:

```javascript
/* --- USER CONFIGURATION (Change these) --- */
const config = {
    targetName: "Sweetheart",
    question: "Will you be my Valentine?",
    thinkingGif: "https://media.giphy.com/media/.../giphy.gif",
    successGif: "https://media.giphy.com/.../giphy.gif",
    dateLocation: "Ulaanbaatar Park",
    dateTime: "Feb 14th @ 1:00 PM"
};
```

### What Each Option Does:

| Option | What It Does | Example |
|--------|-------------|---------|
| `targetName` | The name of your Valentine | `"Sarah"`, `"My Love"`, `"Cutie"` |
| `question` | The question you're asking | `"Will you be my Valentine?"`, `"Go out with me?"` |
| `thinkingGif` | GIF shown during the question | Any Giphy URL |
| `successGif` | GIF shown when they say yes | Any Giphy URL |
| `dateLocation` | Where you'll meet | `"Central Park"`, `"Starbucks Downtown"` |
| `dateTime` | When you'll meet | `"Feb 14th @ 7:00 PM"`, `"Saturday at 6pm"` |

### 🖼️ How to Change GIFs

1. Go to [Giphy.com](https://giphy.com)
2. Search for a GIF you like
3. Click "Share" → "Copy GIF Link"
4. Paste the URL into the config

**Note:** Make sure the URL starts with `https://` and ends with `.gif`

### 🎵 Adding Your Own Music/Sounds (Optional)

If you want custom audio:

1. Add your music file to the same folder as `valentine.html`
2. Name it `music.mp3` for celebration music
3. Name it `minecraft_hurt.mp3` for the "No" button sound

Supported formats: MP3, WAV, OGG

## 🎭 How It Works

### The "No" Button Mechanics
1. **First 5 clicks**: The "Yes" button grows bigger each time
2. **After 5 clicks**: The "No" button starts teleporting around the screen
3. **Sound effect**: Plays a sound each time "No" is clicked

### The "Yes" Button
- Triggers celebration music
- Shows floating hearts animation
- Displays your custom success message with date details

## 📂 Project Structure

```
valentine-proposal/
│
├── valentine.html          # Main file (customize this!)
├── astor_logo.png         # Your logo (optional)
├── music.mp3              # Celebration music (optional)
├── minecraft_hurt.mp3     # "No" button sound (optional)
└── README.md              # This file
```

## 🌐 Hosting Your Page

### Option 1: GitHub Pages (Free & Easy)
1. Create a GitHub account
2. Create a new repository
3. Upload `valentine.html`
4. Go to Settings → Pages
5. Select "main" branch and save
6. Your page will be live at `https://yourusername.github.io/repository-name`

### Option 2: Netlify (Drag & Drop)
1. Go to [Netlify.com](https://netlify.com)
2. Drag your folder onto the site
3. Get an instant live URL

### Option 3: Share the File
- Just send `valentine.html` via email/messaging
- They can open it in any browser

## 🎨 Advanced Customization

### Changing Colors

Find the `:root` section at the top of the CSS:

```css
:root {
    --primary-pink: #ff4d6d;      /* Main pink color */
    --secondary-pink: #ff85a1;     /* Light pink */
    --soft-white: #fff0f3;         /* Background */
    --text-color: #590d22;         /* Text color */
}
```

Use a [color picker](https://htmlcolorcodes.com/) to choose new colors.

### Changing Button Text

The buttons say "Yes" and "No" by default. To change them, find this in the HTML:

```html
<button id="yesBtn">Yes</button>
<button id="noBtn">No</button>
```

Change to whatever you like:
```html
<button id="yesBtn">Absolutely!</button>
<button id="noBtn">Maybe...</button>
```

### Adjusting Animation Speed

In the CSS, find the hearts animation:

```css
heart.style.animationDuration = (2 + Math.random() * 2) + 's';
```

Change the numbers to make hearts float faster or slower.

## 📱 Mobile Responsive

The page automatically adjusts for:
- Phones (small screens)
- Tablets (medium screens)  
- Desktops (large screens)

## ❓ Troubleshooting

**Q: The GIF doesn't show up**
- Make sure the URL is correct and starts with `https://`
- Try a different GIF from Giphy

**Q: Music doesn't play**
- Some browsers block autoplay. The user might need to click to enable sound
- Make sure your audio file is in the same folder

**Q: The page looks broken**
- Make sure you didn't accidentally delete any quotes `"` or commas `,`
- Check that all opening tags have closing tags

**Q: Changes aren't showing**
- Clear your browser cache (Ctrl+Shift+R or Cmd+Shift+R)
- Make sure you saved the file

## 💡 Tips

- Test the page yourself before sending it
- Choose GIFs that match your Valentine's personality
- Make sure the date/time/location are correct!
- Consider adding a personal touch in the success message
- Keep it light and fun - don't stress if they say no (though the button makes it hard to! 😄)

## 🤝 Credits

Created by: Astor  
Instagram: [@astor.stem](https://instagram.com/astor.stem)  
Email: astor.stem@gmail.com

## 📄 License

Feel free to use this project for your own Valentine's proposal! Just keep the credits in the footer. ❤️

---

### 🌟 Made with love! Good luck with your proposal! 🌟

---

## 🆘 Need Help?

If you're stuck or have questions:
1. Check the troubleshooting section above
2. Open an issue on this GitHub repository
3. Email me at astor.stem@gmail.com

**Happy Valentine's Day! 💕**
