# 🎮 Guigaum Steam Analytics

A visually rich web dashboard that displays **real-time Steam profile statistics** using the official Steam Web API, enhanced with fun comparisons, projections, and interactive UI elements.

This project was built as a front-end focused application to explore API consumption, caching strategies, UI/UX design, and resilience against network and CORS limitations.

---

## 🚀 Features

- 🔍 **Real-time Steam profile data**
- 🎮 Recently played games (last 2 weeks)
- ⏱️ Total playtime calculations and projections
- 📊 Daily, weekly, and monthly playtime insights
- 🧠 Fun and playful statistics comparisons
- 🟢 Live online / in-game / offline status
- 💾 Local cache system to reduce API requests
- 🌐 Automatic CORS proxy fallback system
- 📱 Fully responsive design
- 🌙 Theme toggle (Light / Dark ready)
- ⚠️ Offline & API failure fallback data

---

## 🧩 Technologies Used

- **HTML5**
- **CSS3** (Custom design, animations, responsive layout)
- **Vanilla JavaScript**
- **Steam Web API**
- **LocalStorage (Cache System)**
- **Font Awesome Icons**

No frameworks were used — everything is built with pure JavaScript to better understand core front-end concepts.

---

## 🗂️ How It Works

1. Fetches profile and game data from the **Steam Web API**
2. Uses **multiple CORS proxies** as fallback to avoid request blocking
3. Stores API responses in **localStorage** with TTL (time-to-live)
4. Automatically:
   - Uses cached data when valid
   - Falls back to sample data if the API is unavailable
5. Processes raw data into meaningful statistics and UI components

---

## 🔐 API & Security Notes

> ⚠️ **Important:**  
This project uses a Steam API key directly in the front-end **for educational and personal use only**.

For production environments:
- Never expose API keys in client-side code
- Use a backend or serverless function as a proxy

---

## 📦 Cache Strategy

| Data Type | Cache Duration |
|---------|----------------|
| Profile | 5 minutes |
| Games | 10 minutes |
| Stats | 15 minutes |

Users can manually clear the cache via the interface.

---

## 🖥️ Live Preview

🔗 **Steam Profile:**  
https://steamcommunity.com/profiles/76561198023046376/

🔗 **Repository:**  
https://github.com/jow320/guigaumhours

---

## 🎯 Purpose of the Project

This project was created to:

- Practice real API consumption
- Improve front-end architecture and state handling
- Learn how to deal with unreliable external services
- Build a polished UI using only native web technologies
- Explore caching and performance optimization

---

## 🛠️ Possible Improvements

- Backend proxy for API security
- Internationalization (i18n)
- Charts with Canvas or SVG
- User-configurable Steam ID
- PWA offline-first enhancements

---

## 📄 License

This project is for **educational and personal use**.  
Steam and all related assets are trademarks of **Valve Corporation**.

---

Made with ❤️ and ☕ by **Victor Estevan**
