# The Kentucky Homestead

## Overview
The Kentucky Homestead is a static website that provides Bible-based audiobook adventures for kids (KJV), along with educational resources like quizzes and coloring pages. The project aims to support a homestead for homeless children in Kentucky.

## Project Type
Static HTML/CSS website served via Python HTTP server

## Current State
✅ Website fully functional and running on Replit
✅ Server configured on port 5000
✅ Deployment configured for autoscale
✅ All pages accessible and working

## Project Structure
```
/
├── index.html              # Main landing page
├── server.py              # Python HTTP server (serves on 0.0.0.0:5000)
├── assets/
│   └── styles.css         # Global styles
├── stories/               # Stories listing page
├── donate/                # Donation page
├── contact/               # Contact page
├── legal/
│   ├── privacy/          # Privacy policy
│   └── terms/            # Terms of service
├── img/                   # Images
├── audio/                 # Audio files directory (add episode MP3s here)
└── downloads/             # PDF downloads (quizzes, coloring pages)
```

## Running the Project
The website runs automatically via the Server workflow:
- **Command**: `python3 server.py`
- **Port**: 5000
- **Host**: 0.0.0.0 (configured for Replit proxy)

## Missing Content (To Be Added)
The following files are referenced but not yet present:
- `/audio/episode1-part1.mp3` - Episode 1 audio file
- Additional audio files for future episodes

Note: Quiz and coloring page PDFs are already in the downloads folder.

## External Integrations Needed
The website includes placeholder links that need to be configured:
1. **Email Service**: Line 56 of `index.html` - `https://YOUR_EMAIL_SERVICE_ENDPOINT`
2. **Payment Processing**: `donate/index.html` - Stripe payment link `https://buy.stripe.com/YOUR_PAYMENT_LINK`
3. **SMS Alerts**: Phone number placeholder on main page for episode alerts

## Technologies
- HTML5
- CSS3 (custom dark theme with golden accents)
- Python 3.11 (SimpleHTTPServer for serving static files)
- No build process required

## Deployment
Configured for Replit autoscale deployment:
- Static website that scales based on traffic
- No database required
- Runs `python3 server.py` in production

## Recent Changes (October 20, 2025)
- Initial Replit setup completed
- Created Python HTTP server with cache-control headers
- Configured workflow and deployment
- Organized PDF files into downloads directory
- Created audio directory for future episodes
