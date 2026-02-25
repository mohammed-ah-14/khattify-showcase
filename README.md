## Khattify – Arabic Calligraphy Generation Web Application

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)

---

### What This Is?

**Khattify** is an event-based web application I built (commissioned by my college) to generate personalized Arabic calligraphy artwork in real time for live event attendees.

Instead of pre-printing generic designs, attendees could enter their names and instantly receive beautifully rendered Arabic calligraphy — complete with a QR code to download their artwork.

**The Problem**: Creating personalized calligraphy for large live events is slow, manual, and hard to scale.  
**My Solution**: A real-time web app that generates stylized Arabic calligraphy, stores the artwork in the cloud, and provides instant access via QR codes.

---

### Why I Built This?

The college wanted an interactive cultural-tech experience for an event. I saw this as an opportunity to combine:

- Arabic typography & design
- Real-time web technologies
- Cloud storage
- QR-based digital distribution

It was also a great challenge in performance optimization since the app needed to handle multiple users at the same time during a live event.

---

### Features

- **Bilingual name translation** (English → Arabic)
- **Multiple calligraphy styles** (Thuluth, Aref)
- **Dynamic real-time rendering**
- **Instant PNG generation**
- **Unique QR code creation** for each design
- **Cloud storage via Supabase**
- **Live event-ready deployment**
- **Responsive design** (works on tablets, laptops, kiosks)

---

### How It Works

1. User enters their name in English or Arabic
2. App translates (if needed) and stylizes the name
3. Selected font (Thuluth or Aref) is applied
4. Artwork is dynamically rendered as a high-quality PNG
5. PNG is uploaded to Supabase Storage
6. A unique QR code is generated linking to the hosted image
7. User scans QR to download or share their artwork

---

### What I Used

- **Frontend**: Flutter (Dart)
- **Backend / Database**: Supabase
- **Cloud Storage**: Supabase Storage Buckets
- **QR Code Generation**: Dart QR libraries
- **Deployment**: Vercel (optimized for concurrent event traffic)
- **Version Control**: GitHub

---

### Screens (Conceptual Flow)

#### Name Input Screen
*Users enter their name and select calligraphy style*

#### Calligraphy Preview
*Real-time preview with dynamic font rendering*

#### QR Code Screen
*Unique QR code generated for instant download*

---

### What Worked Well

- Handled concurrent event usage smoothly
- Real-time generation felt instant to users
- QR-based distribution reduced printing dependency
- Attendees loved the personalized cultural touch
- Clean UI made it easy for non-technical users

---

### Challenges I Faced

#### 1. Arabic Typography Rendering
Rendering Arabic calligraphy correctly — especially with stylistic fonts like Thuluth — required careful handling of text direction (RTL) and font shaping.

#### 2. Translation Accuracy
Ensuring English-to-Arabic name transliteration looked natural and culturally appropriate required testing and refinement.

#### 3. Real-Time Performance
Because this was used during a live event, performance optimization was critical. I had to:
- Optimize image rendering
- Reduce upload latency
- Prevent duplicate file generation
- Handle concurrent requests smoothly

#### 4. QR Code + Cloud Sync
Making sure every generated QR code reliably mapped to the correct stored PNG required careful naming conventions and secure storage handling.

#### 5. Deployment Stability
Since it was event-based, downtime wasn’t an option. Deployment on Vercel had to be tested thoroughly under simulated load.

---

### What I Learned

- Advanced Flutter rendering techniques
- Handling RTL (Right-To-Left) languages properly
- Cloud storage architecture with Supabase
- Generating and serving static assets dynamically
- Event-ready deployment strategy
- Performance optimization for live environments
- Designing for non-technical users in public settings

---

### If I Had More Time...

Some ideas for future improvements:

- More traditional Arabic font styles
- Custom color palettes & backgrounds
- SVG export support (for professional printing)
- Social media sharing integration
- Offline fallback mode
- Analytics dashboard for event organizers
- Batch export for large print runs

---

### About This Repo

This is a showcase repository.  
The full production code is private since it was developed for a college-commissioned live event.

I’m happy to discuss the architecture, rendering approach, or deployment strategy if you're interested!

---

### Reflections

Khattify was one of the most unique projects I’ve built — blending culture, design, and engineering into a live interactive experience.

It pushed me beyond standard CRUD applications into:
- Real-time rendering
- Performance under pressure
- UX design for public events
- Arabic-first digital design

Seeing attendees scan their QR codes and share their personalized calligraphy made the entire project worth it.

---

### Questions or Feedback?

Feel free to reach out!

📧 **Email**: mohammed.abdulharis@outlook.com

---
Spring 2026
