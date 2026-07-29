# AI Literacy — Learn, Use Safely, Verify

A free, interactive web-based learning experience designed to help middle schoolers (and anyone new to AI) understand the fundamentals of artificial intelligence, use it responsibly, and evaluate claims critically.

---

## 📚 What This Is

This is a **single-page HTML5 application** that guides learners through three core activities:

1. **What is AI?** — Demystify AI through interactive quiz questions
2. **Use Safely & Ethically** — Navigate real-world scenarios and ethical dilemmas
3. **Verify Before You Trust** — Learn to spot red flags and fact-check AI-generated claims

No installation required. Just open the page in any modern browser and start learning. Your progress is saved locally on your device.

---

## 🚀 Quick Start

### For Users
Simply visit the hosted page (via GitHub Pages or any web server) and click through the three activities. No account, no login, no tracking—just learning.

**Browser Compatibility:**
- Chrome/Edge (v90+)
- Firefox (v88+)
- Safari (v14+)
- Mobile browsers (iOS Safari, Chrome Mobile)

### For Developers / Self-Hosting

1. **Clone the repo:**
   ```bash
   git clone https://github.com/[your-org]/ai-literacy.git
   cd ai-literacy
   ```

2. **Open locally:**
   ```bash
   # On macOS/Linux
   open index.html
   
   # On Windows
   start index.html
   ```

3. **Deploy to GitHub Pages:**
   - Push to your repo
   - Go to **Settings → Pages**
   - Select `main` branch as source
   - Your page will be live at `https://[your-org].github.io/ai-literacy`

4. **Deploy elsewhere:**
   - Copy `index.html` to any web server
   - No build step, no dependencies, no configuration needed

---

## 🎯 Learning Outcomes

By completing all three activities, learners will be able to:

- **Define AI** in plain language and recognize how it differs from human intelligence
- **Identify AI use cases** in their daily lives (predictive text, recommendation systems, etc.)
- **Evaluate ethical dilemmas** involving AI, including issues of plagiarism, privacy, and misuse
- **Spot red flags** in AI-generated claims (extreme numbers, missing sources, oversimplification)
- **Apply verification techniques** to fact-check information before trusting it
- **Understand the role of humans** in designing, building, and training AI systems

---

## 📋 Technical Details

### Architecture
- **Single File:** Everything is in `index.html` (HTML + CSS + JavaScript)
- **No External Dependencies:** No CDNs, npm packages, or build tools required
- **Responsive Design:** Mobile-first approach; works from 320px to 2560px
- **Accessibility:** Keyboard navigation, focus indicators, respects `prefers-reduced-motion`

### Data & Privacy
- **Local Storage Only:** Progress is saved to your device's localStorage; no data is sent to servers
- **No Tracking:** No analytics, no cookies, no user profiling
- **Clearing Data:** localStorage is cleared when you clear your browser cache

### Color Palette
| Element | Color | Hex |
|---------|-------|-----|
| Background | Deep Navy | `#0a1628` |
| Card Background | Navy Light | `#1a2a42` |
| Accent (Interactive) | Cyan | `#00d9ff` |
| Accent (Warning) | Red | `#ff3366` |
| Accent (Correct) | Green | `#4ade80` |
| Text Primary | Near-White | `#f0f4f8` |
| Text Secondary | Muted Gray | `#a0aec0` |

### Typography
- **Headlines:** System font stack (San Francisco, Segoe UI, Roboto, etc.) at 700 weight
- **Body:** Same system stack for maximum legibility and performance
- **Base Font Size:** 16px on mobile, 18px on desktop
- **Line Height:** 1.6 for body text, optimized for readability

### Progress Tracking
Each activity completion is tracked via localStorage. When all three activities are finished:
- A completion ring fills with cyan
- A celebration message appears
- Progress persists across browser sessions (until localStorage is cleared)

---

## 🛠️ How to Modify & Extend

### Change Colors
Edit the CSS variables at the top of the `<style>` block:
```css
:root {
    --navy: #0a1628;           /* Change primary background */
    --cyan: #00d9ff;            /* Change interactive accent */
    --red: #ff3366;             /* Change warning accent */
    --green: #4ade80;           /* Change success accent */
    /* ... etc */
}
```

### Edit Activity Content
Find the activity card in the HTML (search for `activity-card`). Update:
- Activity title (in the `.activity-title`)
- Activity description (in the `.activity-description`)
- Quiz questions or scenario text
- Feedback messages

### Add a New Activity
1. Copy an existing activity card (e.g., Activity 1)
2. Change the activity number and title
3. Add your content (quiz questions, scenarios, etc.)
4. Update the `completeActivity()` function in the JavaScript to track it
5. Update localStorage logic to include `activity4: false`

### Add External Links
Keep them minimal and focused. Example:
```html
<a href="https://example.com" target="_blank">Link Text</a>
```

---

## 📖 Learning Resources Referenced

This curriculum is informed by:
- **NIST AI Risk Management Framework** — AI governance and risk mitigation
- **OWASP LLM Top 10** — Security risks specific to large language models
- **ISO/IEC 42001** — AI Management Systems standard
- **MITRE ATLAS** — Adversarial tactics, techniques, and common knowledge (AI-focused)
- **EU AI Act & AI Executive Order** — Regulatory and ethical frameworks

---

## 🤝 Contributing

This is an open resource. If you'd like to:
- **Report a bug:** Open an issue with a clear description
- **Suggest an activity:** Describe the learning goal and scenario
- **Translate the page:** Create a new branch and submit a pull request
- **Improve accessibility:** Feedback on keyboard navigation, color contrast, etc.

Please include context and testing results with any contributions.

---

## 📜 License

This project is released under the **MIT License**. You're free to use, modify, and distribute it for educational purposes. Attribution appreciated but not required.

**Created for:** Middle schoolers and anyone new to AI
**First Released:** 2026
**Maintained by:** Frank Stevens

---

## 🔍 FAQ

**Q: Why no animations?**  
A: There are subtle animations, but they respect `prefers-reduced-motion` to avoid distraction or accessibility issues.

**Q: Can I use this offline?**  
A: Yes! Once the page loads, it works entirely offline. Just save the HTML file locally.

**Q: Can I modify this for my classroom?**  
A: Absolutely. Make a copy, change the content, and share it with your students. No permission needed.

**Q: Will my progress sync across devices?**  
A: No. Progress is stored locally on each device. This is intentional for privacy.

**Q: How do I clear progress?**  
A: Clear your browser's cache/localStorage, or open the page in an incognito window.

---

## 📝 Version History

- **v1.0** (2026) — Initial release with 3 core activities, localStorage progress tracking, and responsive design

---

## 💬 Questions or Feedback?

Open an issue on GitHub or reach out directly. Your feedback helps make this resource better for everyone.

---

**Remember:** AI literacy isn't just about understanding how AI works—it's about understanding yourself as a critical thinker and ethical user of technology.
