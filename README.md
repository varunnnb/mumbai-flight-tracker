
A real-time Heads-Up Display (HUD) web application that visually tracks aircraft near Mumbai Airport, fetching live data from the OpenSky Network API and displaying it with smooth animations and a futuristic interface.

**Live Demo:** [https://mumbai-flight.netlify.app/](https://mumbai-flight.netlify.app/)

---

## Overview

This project is a visual flight tracker built using only HTML, Tailwind CSS, and vanilla JavaScript — no backend required.  
It displays live flight details such as:

- Airline and Callsign  
- Origin Airport (with city and country lookup from `codes.csv`)  
- Altitude  
- Ground Speed  
- Heading  
- Vertical Speed  
- Aircraft Model  

The design replicates a futuristic HUD (Heads-Up Display) using GSAP animations, blurred glass panels, and a live starfield background for visual depth.

---

## Tech Stack

- HTML5  
- Tailwind CSS (for utility-first styling)  
- GSAP (GreenSock Animation Platform) for animations  
- Font Awesome for icons  
- OpenSky Network API – real-time aircraft data  
- HexDB API – aircraft model details  
- CSV Lookup (codes.csv) – maps airport ICAO codes to readable city and country names  

---

## Features

- Live aircraft tracking within the Mumbai region (using bounding box coordinates)  
- Animated plane flying across the top of the screen  
- Dynamic starfield background created using JavaScript  
- Glassmorphism-inspired HUD panels  
- Smooth data transitions using GSAP  
- Auto-refresh every 20 seconds with API rate-limit handling  

---

## How It Works

1. The app queries the OpenSky API for aircraft currently in the Mumbai airspace.  
2. The first detected aircraft’s ICAO code is used to:  
   - Fetch origin airport details (via OpenSky + `codes.csv`).  
   - Fetch aircraft model info (via HexDB API).  
3. The dashboard then animates and displays all real-time flight data in a stylized HUD.  

---

## Preview

Visit the live deployed version here:  
[https://mumbai-flight.netlify.app/](https://mumbai-flight.netlify.app/)


<img width="1680" height="795" alt="Screenshot (176)" src="https://github.com/user-attachments/assets/3b390884-37a9-466a-82b4-75c4e7c89486" />

<img width="1680" height="800" alt="Screenshot (111)" src="https://github.com/user-attachments/assets/4cd9ea92-0d47-4cfb-b3b8-798e6e1c74bf" />


---

## Learning Outcomes

- Gained hands-on experience integrating public APIs (OpenSky & HexDB).  
- Learned Tailwind CSS and glassmorphism styling.  
- Practiced smooth UI animations using GSAP.  
- Enhanced data handling and live updates in frontend-only projects.  

---

## Notes

- Due to API rate limits, updates may pause occasionally (handled automatically).  
- Sometimes aircraft data may not include origin info (shown as “Origin Not Reported”).   

---

## License

This project is made purely for learning and educational purposes.  
No commercial use or ownership is claimed over the data sources or external APIs.  
All trademarks, API data, and content belong to their respective owners.  

---

