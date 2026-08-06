# AI & Security Literacy — Complete Learning Path

A free, interactive web-based learning experience designed to help middle schoolers (and anyone new to AI) understand AI fundamentals, stay safe online, think critically about claims, and validate responses using hands-on practice.

---

## 📚 What This Is

This is a **complete learning suite** with five interconnected activities:

1. **What is AI?** — Interactive quiz demystifying artificial intelligence
2. **Use Safely & Ethically** — Navigate real-world scenarios and ethical dilemmas
3. **Verify Before You Trust** — Learn to spot red flags and fact-check claims
4. **Online Safety** — Five subsections covering passwords, phishing, privacy, device security, and AI-specific threats; includes incident response framework
5. **Hands-On Validation** — Use Claude directly to ask questions, validate responses, and practice critical thinking

No installation required. Just open the pages in a browser and start learning. Progress is saved locally on your device.

---

## 🎯 Learning Arc

The five activities build on each other:

- **Activities 1–3** teach foundational AI literacy: what AI is, how to use it ethically, and how to verify claims
- **Activity 4** expands to real-world security: protecting passwords, spotting phishing, managing privacy, securing devices, and understanding AI-specific threats
- **Activity 5** is where you practice: interact with Claude directly, paste responses, and validate them using structured checklists

**By the end**, you'll understand AI, protect yourself online, think critically about information, and validate what you see before trusting it.

---

## 🚀 Quick Start

### For Users

Visit the site and start with the home page (index.html). The landing page explains the full journey and lets you navigate to each activity.

**Browser Compatibility:**
- Chrome/Edge (v90+)
- Firefox (v88+)
- Safari (v14+)
- Mobile browsers (iOS Safari, Chrome Mobile)

### For Activity 5 (Hands-On Validation)

**You'll need access to Claude.** Here's the workflow:

1. **Open two tabs:**
   - Tab 1: This learning site
   - Tab 2: Claude (your mentor's account at claude.ai)

2. **For each task in Activity 5:**
   - Copy the suggested prompt from the task card
   - Paste it into Claude
   - Copy Claude's full response
   - Paste it back into the task card on this site
   - Use the validation checklist to evaluate the response

3. **The key:** You're learning to think critically about AI output. Not all AI responses are correct or complete. Your job is to verify, question, and validate.

### For Developers / Self-Hosting

1. **Clone the repo:**
   ```bash
   git clone https://github.com/[your-org]/ai-literacy.git
   cd ai-literacy
   ```

2. **File structure:**
   ```
   /ai-literacy/
   ├── index.html              (landing/gateway page)
   ├── activity-4.html         (online safety)
   ├── activity-5.html         (hands-on validation)
   ├── README.md               (this file)
   └── [original activities 1–3 also on index.html]
   ```

3. **Open locally:**
   ```bash
   # On macOS/Linux
   open index.html
   
   # On Windows
   start index.html
   ```

4. **Deploy to GitHub Pages:**
   - Push to your repo
   - Go to **Settings → Pages**
   - Select `main` branch as source
   - Your page will be live at `https://[your-org].github.io/[repo-name]/ai-literacy/`

5. **Deploy elsewhere:**
   - Copy all `.html` and `.md` files to any web server
   - No build step, no dependencies, no configuration needed

---

## 📋 Activity Breakdown

### Activity 1: What is AI? (5 min)
- Three quiz questions testing understanding of AI fundamentals
- Immediate feedback on each answer
- Covers: AI as pattern-finding, not magic; AI as human-built systems; examples from daily life

### Activity 2: Use Safely & Ethically (7 min)
- Three scenario cards with branching choices
- Feedback on safe vs. risky decisions
- Covers: essay writing ethics, personal data privacy, deepfakes and impersonation

### Activity 3: Verify Before You Trust (8 min)
- Red flag framework for evaluating claims
- Hands-on checklist to identify false information
- Teaches: extreme numbers, unrealistic timelines, missing sources, oversimplification

### Activity 4: Online Safety (15–20 min)
- Five subsections (tabbed interface):
  - **Passwords:** Password hygiene, password managers, 2FA
  - **Phishing:** Red flags for social engineering, verification techniques
  - **Privacy:** Data management, social media settings, what to share online
  - **Device Security:** Updates, antivirus, screen locks, device hardening
  - **AI Threats:** Deepfakes, AI-generated social engineering, prompt injection awareness
- **Incident Response Framework:** Five-step process for when things go wrong (STOP → Tell Adult → Identify → Act → Learn)

### Activity 5: Hands-On Validation (20–30 min)
- Four guided tasks using Claude:
  1. **Factual Validation:** Verify historical facts against trusted sources
  2. **Quality Assessment:** Evaluate usefulness and depth of advice
  3. **Spotting Gaps:** Identify missing nuance, incomplete context, oversimplification
  4. **Real-World Verification:** Cross-reference with Google, compare results
- Each task includes a validation checklist and reflection prompt
- Teaches: "human in the loop" thinking, critical evaluation, source verification

---

## 🎯 Learning Outcomes

By completing all five activities, learners will be able to:

- **Define AI** in plain language and recognize how it differs from human intelligence
- **Identify AI use cases** in daily life
- **Evaluate ethical scenarios** involving AI, including plagiarism, privacy, and misuse
- **Spot red flags** in AI-generated claims (extreme numbers, missing sources, oversimplification)
- **Apply verification techniques** to fact-check information
- **Protect personal data** online (passwords, phishing awareness, privacy settings)
- **Understand device security** basics (updates, antivirus, screen locks)
- **Recognize AI-specific threats** (deepfakes, social engineering, prompt injection)
- **Respond to security incidents** with a structured five-step framework
- **Validate AI responses** using critical thinking and human judgment
- **Think like a security professional** by questioning, verifying, and validating information

---

## 📋 Technical Details

### Architecture
- **Multiple Files:** `index.html`, `activity-4.html`, `activity-5.html` (activities 1–3 are embedded in index.html)
- **No External Dependencies:** No CDNs, npm packages, or build tools required
- **Responsive Design:** Mobile-first approach; works from 320px to 2560px
- **Accessibility:** Keyboard navigation, focus indicators, respects `prefers-reduced-motion`
- **localStorage:** Progress is saved on the user's device; no data sent to servers

### Data & Privacy
- **Local Storage Only:** All progress data stays on the user's device
- **No Tracking:** No analytics, no cookies, no user profiling
- **Clearing Data:** localStorage is cleared when the user clears their browser cache

### Color Palette
| Element | Color | Hex | Use |
|---------|-------|-----|-----|
| Background | Deep Navy | `#0a1628` | Primary background; trust, seriousness |
| Card Background | Navy Light | `#1a2a42` | Activity containers |
| Accent (Interactive) | Cyan | `#00d9ff` | Interaction, curiosity, learning |
| Accent (Caution/Security) | Red | `#ff3366` | Warnings, security concerns, incident response |
| Accent (Safe/Correct) | Green | `#4ade80` | Safe practices, correct choices, completion |
| Text Primary | Near-White | `#f0f4f8` | Body text, high contrast |
| Text Secondary | Muted Gray | `#a0aec0` | Supporting text, metadata |

### Typography
- **Headlines:** System font stack (San Francisco, Segoe UI, Roboto, etc.) at 700 weight, all-caps for action headers
- **Body:** Same system stack for legibility and performance
- **Base Font Size:** 16px on mobile, 18px on desktop
- **Line Height:** 1.6 for body text, optimized for readability

### Progress Tracking
- Activities 1–5 are tracked via localStorage
- A progress ring on the landing page fills as activities are completed
- Progress persists across browser sessions (until localStorage is cleared)
- Each activity can be revisited and re-completed

---

## 🛠️ How to Modify & Extend

### Change Colors
Edit the CSS variables at the top of each `.html` file:
```css
:root {
    --navy: #0a1628;           /* Primary background */
    --cyan: #00d9ff;            /* Interactive accent */
    --red: #ff3366;             /* Security/caution accent */
    --green: #4ade80;           /* Safe/correct accent */
    /* ... etc */
}
```

### Edit Activity Content
Find the activity card or section in the HTML and update:
- Activity titles
- Task descriptions
- Quiz questions or scenario text
- Validation criteria
- Feedback messages

### Add a New Activity
1. Create a new `.html` file (e.g., `activity-6.html`)
2. Copy the structure from an existing activity file
3. Update colors, content, and validation checklists
4. Add a link in `index.html` to the new activity
5. Update the progress tracking logic

### Customize for Your Context
- Replace "Claude" references with your specific AI tool name
- Add your school/organization's name or logo (in header comments or footer)
- Adjust scenarios to reflect your student population's interests or challenges
- Add or remove subsections from Activity 4 as needed

---

## 📖 Learning Frameworks Referenced

This curriculum is informed by:
- **NIST AI Risk Management Framework** — AI governance and risk mitigation
- **OWASP LLM Top 10** — Security risks specific to large language models
- **ISO/IEC 42001** — AI Management Systems standard
- **MITRE ATLAS** — Adversarial tactics, techniques, and common knowledge (AI-focused)
- **MITRE ATT&CK** — Adversary tactics and techniques (cyberattack framework)
- **EU AI Act** — Regulatory framework for AI in Europe
- **Executive Order on AI** — U.S. policy on AI governance and safety

---

## 🤝 Contributing

This is an open resource. If you'd like to:
- **Report a bug:** Open an issue with a clear description
- **Suggest an activity:** Describe the learning goal and scenario
- **Translate:** Create a new branch and submit translations
- **Improve accessibility:** Feedback on keyboard navigation, color contrast, etc.
- **Add scenarios:** Contribute realistic, age-appropriate scenarios for Activity 2 or 4

Please include context and testing results with any contributions.

---

## 📜 License

This project is released under the **MIT License**. You're free to use, modify, and distribute it for educational purposes. Attribution appreciated but not required.

**Created for:** Middle schoolers and anyone new to AI and cybersecurity
**First Released:** 2026
**Maintained by:** Frank Stevens

---

## 🔍 FAQ

**Q: Why do I need to copy/paste Claude's responses into the page?**  
A: It keeps the learning focused on *you* validating and thinking critically. You're not relying on automation; you're practicing human judgment.

**Q: Can I use this offline?**  
A: Yes! Once the pages load, they work entirely offline. Just save the HTML files locally.

**Q: Can I modify this for my classroom?**  
A: Absolutely. Make a copy, change the content, and share with your students. No permission needed.

**Q: Will my progress sync across devices?**  
A: No. Progress is stored locally on each device. This is intentional for privacy.

**Q: How do I clear progress?**  
A: Clear your browser's cache/localStorage, or open the page in an incognito window.

**Q: What if a student doesn't have access to Claude?**  
A: Activity 5 is optional. Students can complete Activities 1–4 independently. For Activity 5, an adult needs to provide Claude access (even reading the responses and discussing them counts as validation practice).

**Q: Can I add my own activities?**  
A: Yes. Copy an existing activity's HTML structure and add it as a new file. Update the index page to link to it.

---

## 📝 Version History

- **v2.0** (2026) — Added Activity 4 (Online Safety) and Activity 5 (Hands-On Validation); restructured landing page as narrative gateway
- **v1.0** (2026) — Initial release with 3 core activities, localStorage progress tracking, and responsive design

---

## 💬 Questions or Feedback?

Open an issue on GitHub or reach out directly. Your feedback helps make this resource better for everyone.

---

**Remember:** Digital literacy isn't just about understanding how AI works—it's about understanding yourself as a critical thinker, ethical user, and advocate for safe and responsible technology.
