# Portfolio Website Redesign Prompt for Antigravity

## Starting Point
You are working with the **Oni-Ronin** open-source project by MiladiCode (a 3D samurai game landing page built with Three.js + Vite). Your task is to convert it into a **personal portfolio website** for a Cyber Security professional.

**Original repo:** https://github.com/miladicode823-coder/Oni-Ronin

---

## The Person (Portfolio Owner)

**Name:** SYED SUBHAN HUSSAIN
**Title:** Cyber Security Analyst | IoT & Blockchain Specialist | Software Engineer
**Location:** Bidar, Karnataka, India
**Phone:** +91-8431323178
**Email:** syedsubhanhussain.icb@gmail.com
**LinkedIn:** https://www.linkedin.com/in/syed-subhan-hussain-414675337
**GitHub:** https://github.com/syedsubhanhussain-sih
**Portfolio:** https://syed-subhan-hussain-portfolio.vercel.app

**Education:** BE Computer Science (Cyber Security, IoT & Blockchain), Guru Nanak Dev Engineering College (VTU), Bidar — Class of 2027, CGPA 7.80/10

**Key Skills:** Wireshark, Nmap, Burp Suite, Metasploit, Snort, Nessus, Hydra, John the Ripper, TCP/IP, VPNs, Firewalls, Kali/Ubuntu Linux, C/C++, Java, Python, JavaScript, React, Node.js, FastAPI, MySQL, PostgreSQL, MongoDB, Firebase, Git, Docker

**Key Projects:**
- **DEFENXIA** — Smart India Hackathon Finalist (Team Leader)
- **DEFENXIA Mobile Security App** — Won mini-project competition (₹3,000 prize)

**Practical Experience:** Nmap vulnerability assessments, Wireshark/tcpdump (50+ packet captures), Burp Suite (SQLi/XSS testing), Snort IDS setup, ARP spoofing / MITM simulations

**Leadership:** Led HACKTOBER cyber-awareness event (100+ participants)

**Certifications:** Cisco Networking, Red Hat Linux, Ethical Hacking (Simplilearn), LearnTube, Infosys Springboard, MERN Stack (Zenexis), AWS Cloud Essentials, DevOps + Cloud Security (Cyber Defentech), ADVAYA 2.0

**Achievements:** Smart India Hackathon Finalist, PALS Finals, Class Topper (5th semester)

**Internships (all Cyber Security):** SYNTECXHUB, FUTURE INTERNS, INFOTACT SOLUTIONS

> **Note:** I will also provide a detailed resume PDF. Use it to fill in any additional details, descriptions, and timeline information across the site.

---

## 3D Character Model

I am providing a custom **GLB 3D character model** (`Silent_Shadow` — a person in black shirt with sunglasses, doing a "shh" finger-to-lips pose).

### Requirements:
1. **Replace** the default samurai character with my GLB model
2. The model is **static** (no bones/rigging) — **DO NOT attempt walking animation**
3. Character should **rotate 360° when the user scrolls** (scroll-driven rotation on Y-axis)
4. Character stands in the hero section, centered
5. The character must be **clearly visible** — ensure proper lighting on the model

---

## Theme & Colors

- **Primary theme:** Red and Black (dark, cinematic, gaming aesthetic)
- **Accent red:** `#ff2d12` (for the name text and highlights)
- **Background:** Dark/black with red smoky/ember atmosphere
- Overall vibe: Dark fantasy game landing page → reimagined as a cyber-security professional's portfolio

---

## HERO SECTION (Landing)

### Layout:
1. **Background:** Red smoky/ember background image (provided as `hero-background.webp`) — must be **clearly visible** behind the character, not hidden
2. **3D Character:** Centered, standing, rotating on scroll
3. **Name text:** Giant **"SYED SUBHAN"** (line 1) **"HUSSAIN"** (line 2) text positioned **BEHIND the 3D character**
   - Color: Red (`#ff2d12`)
   - Font weight: **Extra bold / 900**
   - **3D text effect:** Layered text-shadow for depth/extrusion (darker red shadows offset to create 3D look)
   - Size: Large but **responsive** — must look good on BOTH desktop and mobile (not absurdly huge on desktop)
   - The text should appear as a backdrop behind the character, like a cinematic title

4. **Hero statements** (small text, positioned nicely):
   - "Syed Subhan Hussain"
   - "Cyber Security Analyst"

5. **Topbar:**
   - Logo: **"ssh®"** (his initials)
   - Label: "Cyber Security Portfolio"
   - Buttons: "Hire me" (scrolls to footer/contact)

6. **Menu navigation** — update all links to portfolio sections

### ⚠️ IMPORTANT — No Preloader Gate:
- **REMOVE the preloader/enter screen entirely**
- Website must open **directly** when the link is opened — no "Continue" button, no loading gate
- If a loading indicator is needed for 3D assets, make it non-blocking (site should be visible immediately)

---

## SERVICES SECTION (14 Cards in 3D Circular Carousel)

The site has a 3D spiral/circular carousel of cards around a sword. **Replace all 14 cards** with the following portfolio content. Each card has: number, title, category, description, and danger level.

**Card images** are provided in `images/cards/` — each card uses its corresponding image.

| # | Image File | Title | Category | Description |
|---|-----------|-------|----------|-------------|
| 01 | `card-01-cyber-security-analyst.webp` | Cyber Analyst | bounties | Security analyst specializing in threat detection, SOC operations, and incident response. |
| 02 | `card-02-education.webp` | The Education | escorts | BE CSE (Cyber Security, IoT & Blockchain), GNDEC Bidar, VTU — Class of 2027, CGPA 7.80/10. |
| 03 | `card-03-security-arsenal.webp` | Security Arsenal | exorcisms | Wireshark, Nmap, Burp Suite, Metasploit, Snort, Nessus, Hydra, John — the tools of the trade. |
| 04 | `card-04-network-warden.webp` | Network Warden | duels | TCP/IP, VPNs, firewalls, IDS/IPS — hardening networks and catching intrusions in real time. |
| 05 | `card-05-code-and-data.webp` | Code & Data | heists | C, C++, Java, Python, JavaScript, React, Node.js, FastAPI — building secure software and managing data. |
| 06 | `card-06-defenxia-sih.webp` | DEFENXIA SIH | bounties | Team Leader at Smart India Hackathon — built a cyber-security platform as a finalist. |
| 07 | `card-07-defenxia-mobile-app.webp` | DEFENXIA Mobile | exorcisms | Mobile security app that won the mini-project competition (₹3,000 prize). |
| 08 | `card-08-vulnerability-assessment.webp` | Vuln Assessment | duels | Nmap vulnerability scans — mapping open ports, services, and CVEs with remediation reports. |
| 09 | `card-09-packet-hunter.webp` | Packet Hunter | heists | 50+ Wireshark/tcpdump captures analyzed — finding malicious patterns in network traffic. |
| 10 | `card-10-web-security.webp` | Web Security | exorcisms | Burp Suite testing for SQL injection and XSS — securing web applications. |
| 11 | `card-11-intrusion-detection.webp` | Intrusion Detection | duels | Snort IDS with custom rules — simulating ARP spoofing and MITM attacks to strengthen defenses. |
| 12 | `card-12-hacktober-lead.webp` | Hacktober Lead | escorts | Led HACKTOBER cyber-awareness event with 100+ participants. |
| 13 | `card-13-certifications.webp` | Certified Arsenal | bounties | Cisco Networking, Red Hat Linux, Ethical Hacking, AWS Cloud, DevOps+Cloud Security, MERN Stack. |
| 14 | `card-14-achievements.webp` | Proven in Battle | heists | SIH Finalist, PALS Finals, Class Topper (5th sem), 3 cyber-security internships. |

### Card Image Requirements:
- Images must be **BRIGHT and clearly visible** on the cards (not dark/muddy)
- Each card prominently displays its image
- Card text (title, description) must be readable over/near the image

---

## ARSENAL / FEATURES SECTION (5 Features)

Replace the 5 game features with portfolio-themed expertise areas. Each has a title, description, and tags.

**Feature images:** The `images/extra/` folder has 3 additional images (SOC center, blockchain network, IoT devices) — use these for relevant features.

| # | Title | Description | Tags |
|---|-------|-------------|------|
| 01 | Analyze Threats | Threat hunting with Wireshark, Nmap and Burp Suite. Analyzing 50+ packet captures to find malicious patterns before they strike. | Threat hunting, Wireshark, 50+ captures |
| 02 | Secure Networks | Hardening networks with firewalls, VPNs and IDS. Snort rules tuned to catch intrusions in real time across lab systems. | Firewalls, Snort IDS, VPNs |
| 03 | Hunt Vulnerabilities | Nmap vulnerability scans mapping open ports, services and CVEs. Every finding documented with severity and remediation steps. | Nmap scans, CVE mapping, Reports |
| 04 | Defend Systems | Building defenses with Metasploit testing and John the Ripper audits. Simulating ARP spoofing and MITM attacks to strengthen systems. | Pen testing, MITM sims, Hardening |
| 05 | Lead Teams | Led HACKTOBER cyber-awareness event with 100+ participants. Team Leader for DEFENXIA at Smart India Hackathon finals. | 100+ hackers, SIH Finalist, Team lead |

---

## FOOTER SECTION

### Footer Gallery:
Add a **3-image gallery row** in the footer using:
- `images/footer/footer-connect.webp` (Connect/Networking theme)
- `images/footer/footer-portfolio.webp` (Portfolio/Skills showcase theme)
- `images/footer/footer-hire.webp` (Hire/Handshake theme)

Display as 3 equal-sized rounded thumbnails in a row (responsive: stack on mobile).

### Footer Content:
- **Headline:** "Get in touch"
- **Lede:** "Open to Cyber Security Analyst, SOC Analyst and Software Engineer roles. Let's talk."
- **Contact form:** Email input + submit button
- **Link columns:**
  - **Portfolio:** The World, Expertise, Arsenal
  - **Connect:** LinkedIn (real URL), GitHub (real URL), Portfolio (real URL), Email (mailto:)
- **Copyright:** "© 2026 Syed Subhan Hussain. All rights reserved."
- **Footer mark:** Giant "SYED SUBHAN" text (not "ONI RONIN")

---

## TEXT REPLACEMENTS (Remove All Game References)

### Remove "Oni Ronin" from EVERYWHERE:
- ❌ Topbar logo "oni®" → ✅ **"ssh®"**
- ❌ Giant wordmark "ONI RONIN" → ✅ **"SYED SUBHAN"**
- ❌ Preloader "ONI RONIN" → ✅ **"SYED SUBHAN"** (or remove preloader entirely)
- ❌ Footer mark "ONI RONIN" → ✅ **"SYED SUBHAN"**
- ❌ Page title → ✅ **"Syed Subhan Hussain — Cyber Security Portfolio"**
- ❌ Meta description → ✅ Portfolio description
- ❌ "Summoning the oni" → ✅ Remove or replace with "Loading portfolio"

### Remove These Sections:
- ❌ **EDITIONS / Pricing section** — remove entirely (this is a portfolio, not a game store)
- ❌ "Pre-order now" button → ✅ **"Hire me"** (scrolls to footer)
- ❌ "Take the contract" button → ✅ **"Get in touch"** (scrolls to footer)

---

## RESPONSIVE REQUIREMENTS

### The site MUST look good on both Desktop and Mobile:
1. **Hero name text:** Responsive font size — large on mobile, proportionally smaller on desktop (use `clamp()`). Must NOT look absurdly huge on wide screens.
2. **3D character:** Properly sized and positioned on both desktop and mobile
3. **Cards carousel:** Must work on touch (mobile) and mouse (desktop)
4. **Footer gallery:** 3-column on desktop, stacked on mobile
5. **All text:** Readable on both — no overlapping, no cut-off text
6. **Navigation:** Mobile menu must work

### Test on:
- Desktop (1920px wide)
- Mobile (375px wide)
- Tablet (768px wide)

---

## IMAGE PLACEMENT SUMMARY

| Image | Where It Goes |
|-------|---------------|
| `images/cards/card-01` through `card-14` | 14 cards in the 3D circular carousel (Services section) — one image per card |
| `images/footer/footer-connect.webp` | Footer gallery (left) |
| `images/footer/footer-portfolio.webp` | Footer gallery (center) |
| `images/footer/footer-hire.webp` | Footer gallery (right) |
| `images/extra/extra-soc.webp` | Arsenal/Features section (SOC-related feature) |
| `images/extra/extra-blockchain.webp` | Arsenal/Features section (blockchain feature) or About section |
| `images/extra/extra-iot.webp` | Arsenal/Features section (IoT feature) or About section |
| `images/hero-background.webp` | Hero section background (behind 3D character) |

---

## DELIVERABLES

1. Fully working portfolio website (all sections above)
2. Must work when opened directly via URL (no build errors, no stuck loading screens)
3. All 14 card images displaying correctly
4. 3D character loading and rotating on scroll
5. Responsive on desktop + mobile
6. No "Oni Ronin" or game-related text remaining (except where intentionally kept for aesthetic)

---

## TECH NOTES

- Built with **Three.js** + **Vite** (keep the existing build setup)
- 3D character is a **static GLB** (no skeletal animation) — handle gracefully if animation clips are missing
- Card images should have cache-busting (query params or hashed filenames) so updates are visible
- The 3D canvas should ideally be **transparent** so the hero background image and name text show behind the character
