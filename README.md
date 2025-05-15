📊 Live Crypto Price Dashboard
Dashboard Preview
(Example screenshot - replace with your actual screenshot)

🌟 Features
Real-time cryptocurrency prices from CoinGecko API

Interactive 7-day price charts with smooth animations

Multiple cryptocurrency support: Bitcoin (BTC), Ethereum (ETH), Binance Coin (BNB), Solana (SOL)

Responsive design works on mobile and desktop

Automatic error recovery with multiple fallback mechanisms

Self-healing - automatically retries failed requests

Offline-capable with fallback sample data

🚀 Quick Start
Clone the repository:

bash
git clone https://github.com/yourusername/crypto-dashboard.git
Open in browser:

Simply open the index.html file in any modern browser

No server or build step required!

Using GitHub Pages:

Upload to a GitHub repository

Enable GitHub Pages in repository settings

Your dashboard will be live at username.github.io/repository

🛠️ How It Works
Technical Architecture
Frontend: Pure HTML/CSS/JavaScript

Charting: Chart.js

Data Source: CoinGecko API

Error Handling System
Attempts primary API request (5s timeout)

If fails, tries backup endpoint

If still fails, uses locally stored sample data

Shows error message with retry button

Automatic Updates
Data refreshes every 2 minutes

Automatically retries failed requests

📂 File Structure
crypto-dashboard/
└── index.html    # All code in single file (HTML, CSS, JS)
🔧 Customization
Add More Cryptocurrencies
Add a new button in the HTML:

html
<button class="crypto-btn" onclick="fetchData('cardano')">
  <span class="crypto-name">Cardano</span>
  <span class="crypto-symbol">ADA</span>
</button>
Add to the cryptoIds object in JavaScript:

javascript
const cryptoIds = {
  // ...existing currencies
  cardano: 'ADA'
};
Change Design
Modify the CSS variables at the top of the file:

css
:root {
  --primary-color: #6200ea;
  --success-color: #00c853;
  --error-color: #d32f2f;
}
🌐 API Considerations
The dashboard uses CoinGecko's public API:

Free tier has rate limits (10-50 calls/minute)

For heavy usage, consider:

Adding your own proxy server

Implementing client-side caching

Using API keys if needed

🤝 Contributing
Contributions are welcome! Here's how:

Fork the project

Create your feature branch (git checkout -b feature/AmazingFeature)

Commit your changes (git commit -m 'Add some AmazingFeature')

Push to the branch (git push origin feature/AmazingFeature)

Open a Pull Request

📜 License
Distributed under the MIT License. See LICENSE for more information.

✉️ Contact
Your Name - @yourtwitter - youremail@example.com

Project Link: https://github.com/yourusername/crypto-dashboard

🙏 Acknowledgments
CoinGecko for their excellent free API

Chart.js team for the amazing charting library

Inspired by various crypto tracking dashboards

