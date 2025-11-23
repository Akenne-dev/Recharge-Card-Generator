📟 Recharge Card Generator

A simple, interactive, and fully functional recharge card generator and loader built with HTML, CSS, and JavaScript.
This project simulates how airtime recharge cards work — allowing users to:

✅ Generate MTN, Airtel, Glo, and 9Mobile recharge cards
✅ Load (redeem) generated cards
✅ Track used & unused cards
✅ Store data permanently using LocalStorage
✅ Auto-generate & randomize secure 16-digit PINs
✅ Filter and clear transactions (Used, Unused, All)


✨ Features
🔹 1. Network Selection

Users can choose from:

MTN

Airtel

Glo

9mobile

Each network updates the UI with correct colors & branding.


🔹 2. Generate Recharge Cards

Select a preset amount (₦50, ₦100, ₦200, ₦500, ₦1000, ₦2000)

Or enter a custom amount

A secure 16-digit PIN is automatically generated

Cards are saved in localStorage

Example generated PIN:

2384 9921 8842 1130


🔹 3. Load/Recharge Cards

Users can enter a PIN to "load" airtime:

Detects if PIN exists

Prevents loading same PIN twice

Updates card status from Unused → Used


🔹 4. Transactions Table

Displays all generated cards:

S/N	Network	Amount	PIN	Loaded?

With options to filter:

All Cards

Used Cards

Unused Cards


🔹 5. Clear Options

Users can delete:

🗑️ All Used Cards

🗑️ All Unused Cards

🗑️ All Cards

Everything updates in real-time.


🔹 6. Fully Responsive

The entire interface adjusts beautifully for:

Mobile

Tablet

Desktop


🛠️ Technologies Used
Technology	Purpose
HTML5	Structure
CSS3	Styling & responsiveness
JavaScript (ES6)	Logic, validation, localStorage
📂 Project Structure
index.html
│
├── <style> (embedded CSS)
└── <script> (embedded JS)


No external dependencies — fully standalone.


🚀 How It Works
1️⃣ Select a network

The UI updates with the chosen network’s color theme.

2️⃣ Choose or enter an amount

Amount is instantly shown in the balance preview.

3️⃣ Generate card

A PIN is created and stored permanently in localStorage.

4️⃣ Load card

Enter your PIN and the system validates & marks it as used.

5️⃣ View or clear transactions

You can filter cards or wipe entire categories.


💡 Why This Project?

This project is perfect for:

Beginners learning JavaScript logic

Practicing localStorage

UI building with responsive design

Understanding how recharge systems can be simulated


🧪 Demo Functions (Examples)
Generate a 16-digit PIN:
for (let i = 0; i < 16; i++) {
  generatedPin += Math.floor(Math.random() * 10);
  if ((i + 1) % 4 === 0 && i !== 15) generatedPin += " ";
}

Save to Local Storage:
localStorage.setItem("cardsDB", JSON.stringify(database));


🤝 Contributing

Feel free to fork the project and submit improvements or new features.


📄 License

MIT License — free to use, modify, and share.


💗 Author

Made with love by Akennebaby — your favorite tech girl 💅🏽✨
