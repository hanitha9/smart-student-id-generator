
# Smart Student ID Generator

## Overview
This is my submission for the Unity Internship Assignment, a ReactJS-based Smart Student ID Generator built on Replit. It creates customizable ID cards with QR codes, photo previews, and downloadable PNGs, meeting all required features with additional enhancements.

## Features
### Required
1. **Student Data Form**:
   - Fields: Name, Roll Number, Class & Division (dropdown), Allergies (multi-select), Photo Upload (with preview), Rack Number, Bus Route Number (dropdown).
   - Submit button generates the ID card.
2. **Smart ID Card Preview**:
   - Displays student info, photo, allergies, rack/bus route, and a QR code with JSON data.
   - Includes a "Download as PNG" button.
3. **Template Switching**:
   - Dropdown with 4 templates (Classic White, Modern Blue, Emerald Glow, Cosmic Purple).
4. **Persistent Data (Bonus)**:
   - Saves cards to `localStorage`.
   - Drafts tab lists saved cards with download and view options.

### Extras
- Navigation with Home, Generate, View, Drafts, and Customised tabs.
- Customised event IDs with role and event highlighting.
- Persistent school/college logo across tabs.
- Animations using Framer Motion.
- Home page with project info.

## Tech Stack
- **ReactJS**: v18+ with hooks.
- **Libraries**:
  - `qrcode.react`: QR code generation.
  - `html-to-image`: PNG export.
  - `framer-motion`: Animations.
  - `jszip`: Included (unused in final version).
- **Styling**: TailwindCSS.
- **Environment**: Replit.

## Thought Process
1. **Structure**: Used a single `App.jsx` with tab-based navigation for simplicity and clarity.
2. **Form**: Built a reusable form with validation and preview, extending it for customised IDs.
3. **Card Preview**: Designed with TailwindCSS and Framer Motion for polish; added a hidden renderer for Drafts tab downloads.
4. **Templates**: Implemented 4 instead of 2 for variety, using conditional styling.
5. **Persistence**: Leveraged `localStorage` with JSON parsing/stringifying for draft management.
6. **Challenges**: Fixed Drafts tab download by using a ref-based hidden renderer, ensuring DOM updates before `html-to-image` capture.

## How to Run
1. Open in Replit.
2. Run `npm install` to install dependencies.
3. Click "Run" to start the app.
4. Navigate through tabs to test features.

## Video Walkthrough
[Link to your video once recorded]

## Improvements
- Add bulk download for drafts.
- Enhance QR code styling.
- Implement a backend for server-side storage.

Thanks for reviewing my work!
