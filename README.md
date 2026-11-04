# DELIVERY DA! (ஊரு முழுக்க DELIVERY!)
### EVERY STREET HAS A STORY. EVERY DELIVERY IS A CHALLENGE.

**DELIVERY DA!** is an original 2D Tamil Nadu food delivery arcade runner built in HTML5, CSS3, JavaScript (ES6+), and **Phaser 3**.

Ride as a young delivery partner for **NAMMA EXPRESS** through the vibrant, bustling streets of Chennai, Madurai, Coimbatore, Thanjavur, Tiruchirappalli, and Tirunelveli! Weave through notorious Tamil Nadu traffic (government buses, yellow-and-black auto-rickshaws, bikes, milk bicycles, crossing cows, and potholes), collect piping-hot food orders from iconic local mess and tiffin houses, and deliver them to eager customers before the clock runs out!

---

## 🌟 Key Features

1. **2D Arcade Perspective Runner**:
   - 3-lane perspective-based road scaling (OutRun / Road Rash / Subway Surfers style behind-the-rider camera in pure 2D Canvas & Phaser 3).
   - Smooth lane switching, jump mechanics to hop over potholes and speed breakers, acceleration, and braking.

2. **Core 8-State Delivery Architecture**:
   - `ORDER_RECEIVED` ➔ `TRAVELLING_TO_RESTAURANT` ➔ `ARRIVED_AT_RESTAURANT` ➔ `PICKUP_AVAILABLE` ➔ `FOOD_COLLECTED` ➔ `TRAVELLING_TO_CUSTOMER` ➔ `ARRIVED_AT_CUSTOMER` ➔ `DELIVERY_COMPLETED`.
   - Never skips required stages. Impossible to deliver before collecting food. Prevents duplicate claims.

3. **16+ Authentic Fictional Tamil Nadu Restaurants**:
   - *Chennai Tiffin House*, *Madurai Mess*, *Namma Dosa Corner*, *Kovai Biryani Spot*, *Anna Nagar Cafe*, *Mylapore Meals*, *Thanjavur Kitchen*, *Tambaram Parotta House*, *Marina Snacks*, *Namma Idli Kadai*, *Madurai Jigarthanda Corner*, *Nellai Sweets*, *Adyar Veg Kitchen*, and more!
   - Authentic delicacies: Ghee Masala Dosa, Bun Parotta & Salna, Seeraga Samba Biryani, Sambar Idli, Madurai Jigarthanda, Nellai Halwa, Ven Pongal, and Filter Coffee.

4. **Modular Character Customization**:
   - Gender (Male / Female), 4 natural Tamil skin tones, 5 hairstyles.
   - Outfits: *Namma Express Uniform*, *Madras Checks Shirt*, *Tamil Typography Tee*, *Biker Leather Jacket*, *Traditional Veshti & Shirt / Saree*, *Pongal Festival Kurta*.
   - Accessories: Helmets in 4 colors, cool sunglasses, and the insulated Namma Express delivery backpack.
   - **Customizations reflect directly on the actual 2D in-game rider sprite!**

5. **Scooter & Motorcycle Garage**:
   - 6 Unlockable Vehicles:
     1. *Namma Scooter 110* (Classic commuter scooter)
     2. *Super Dio Turbo 125* (High-acceleration sporty scooter)
     3. *Priya Chetak 150* (Vintage heavy-iron scooter with high protection)
     4. *Namma EV Volt 450* (Modern electric smart scooter with responsive handling)
     5. *Namma Splendor 100* (Legendary delivery bike with large parcel capacity)
     6. *Royal Bullet 350* (Heavy thumping cruiser with road presence and top speed)
   - 5 Upgrade Tracks: Top Speed, Acceleration, Handling Agility, Collision Shield, and Parcel Capacity.
   - Custom body color palette selection.

6. **Authentic Tamil Nadu Traffic & Road Obstacles**:
   - *Green & White TNSTC Government Bus* ("அரசு விரைவுப் போக்குவரத்து", route board "18A சென்னை - தாம்பரம்")
   - *Yellow & Black Namma Auto Rickshaw* (signals and switches lanes with rear bumper quotes like "தாய்ப்பால்")
   - *Commuter motorcycles*, *Milkman bicycles with steel milk cans*.
   - Obstacles: Potholes ("ரோட்டு குழி"), Speed Breakers, Police Barricades ("TN POLICE"), Cows crossing peacefully, Indie Street Dogs, and Water Puddles.

7. **Festival Modes & Environments**:
   - **Thai Pongal Rush**: Sugarcane stalks, brass Pongal pots with overflowing milk, colorful Kolam road art, festive music.
   - **Diwali Spark**: Festive decorative serial lights, night sky with fireworks, sweet deliveries.
   - **Temple Festival**: Grand Temple Gopuram backdrop, flower stalls, temple chariot procession.

8. **Dynamic Weather & Time of Day**:
   - Morning, Afternoon sunshine, Golden Hour Sunset, and Night mode with glowing headlights and streetlights.
   - Chennai Monsoon Rain mode with slanted rain particles and wet road reflections.

9. **Power-Ups**:
   - 🛡️ *Helmet Shield* (absorbs 1 collision)
   - 🧲 *Coin Magnet* (attracts nearby coins)
   - ☕ *Filter Coffee Turbo* (invulnerable high-speed zoom)
   - ⏱️ *Time Bonus* (+15 seconds on delivery clock)
   - 💰 *2X Double Coins* (doubles delivery earnings)

10. **Procedural Web Audio API Engine**:
    - Synthesizes realistic 4-stroke engine drone with real-time RPM frequency modulation matching scooter speed!
    - Twin-tone auto horn ("Paamp-paamp!"), coin chimes, parcel collection bell, delivery success fanfare, and festival melody.
    - Speaks original Tamil rider quips using a device-provided Tamil text-to-speech voice when available.
    - Zero external audio files required! 100% offline-ready.

11. **Complete Dual Language Support**:
    - Seamless instant toggle between **English** and **தமிழ் (Tamil)** at any moment.
    - Full Tamil translations for all UI, items, restaurants, areas, and original context-aware rider quips.

12. **LocalStorage Persistence**:
    - Automatically persists coins, unlocked vehicles, upgrade tiers, character styling, achievements, high scores, and settings.

---

## 🎮 Controls

### Desktop Keyboard
- **A / Left Arrow**: Switch to Left Lane
- **D / Right Arrow**: Switch to Right Lane
- **W / Up Arrow**: Jump over Potholes & Speed Breakers
- **S / Down Arrow**: Brake / Decelerate
- **Space**: Honk Scooter Horn / Auto Horn
- **Shift**: Accelerate / Turbo Boost

### Mobile Touch & Gestures
- **Swipe Left / Right**: Switch Lanes
- **Swipe Up**: Jump
- **On-Screen Touch Buttons**: ⬅️ Left, ➡️ Right, 🦘 Jump, 📢 Horn

---

## 🚀 Running Locally

The game runs with zero external runtime dependencies using standard ES modules and Node.js.

### Method 1: Using the built-in server (Fastest)
```bash
node server.js
```
Then open [http://localhost:3000](http://localhost:3000) in your browser.

### Method 2: Using Vite
```bash
npm install
npm run dev
```

---

## 📦 Deployment to Vercel

1. Commit and push the complete project, including `src/`, `index.html`, `phaser.min.js`, `package.json`, and `vite.config.js`.
2. Set the Root Directory to `./`.
3. Set the Build Command to `node build.js` (or `npm run build`).
4. Set the Output Directory to `dist`.

The deployment build uses Node.js directly and does not require Vite to be installed in production.

---

*NAMMA EXPRESS — ஊரு முழுக்க DELIVERY!*
