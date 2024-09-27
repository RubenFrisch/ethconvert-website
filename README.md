# ethconvert-website
# Ether Unit Converter

# Domain: https://ethconvert.xyz/

## Overview
The **Ether Unit Converter** is a simple, user-friendly web application that allows users to convert between various Ethereum-related units (Ether, GWEI, WEI) and fiat currencies (USD, HUF). The application also fetches dynamic Ethereum price and gas data from external APIs, providing real-time price and gas updates.

## Features
- **Ether Unit Converter**: Convert values between Ether, GWEI, WEI, USD, and HUF.
- **Dynamic Ethereum Price**: Fetches the latest Ethereum price in USD using the CoinGecko API.
- **Ethereum Gas Prices**: Fetches live gas prices (low, average, high) using the Etherscan Gas Oracle API.
- **Auto-Refresh**: Automatically refreshes Ethereum price every 300 seconds and gas prices every 30 seconds.
- **Copy to Clipboard**: Each input field has a "Copy" button to quickly copy the converted value to the clipboard.
- **Countdown Timer**: Shows countdown timers for the next price and gas data updates.
- **Responsive Design**: The app is optimized for different screen sizes, providing a great user experience on both desktop and mobile.

## Technologies Used
- **HTML**: The structure and content of the page.
- **CSS**: Styling for the page to provide an elegant, dark-themed user interface.
- **JavaScript**: Functionality to handle the unit conversions, fetch data from external APIs, and manage dynamic updates.
- **CoinGecko API**: Fetches the current Ethereum price in USD and the USD to HUF exchange rate.
- **Etherscan API**: Retrieves current gas prices (Safe, Propose, and Fast).

## How It Works
1. **Unit Conversion**: Users can input values into any of the Ether, GWEI, WEI, USD, or HUF fields, and the app will automatically update the other fields with the converted values.
   - **Ether to GWEI/WEI**: Converts Ether to its smaller units.
   - **USD/HUF Conversion**: Converts Ether units to their fiat currency equivalents using the latest price and exchange rates.
   
2. **Dynamic Price Updates**:
   - The app fetches the latest Ethereum price from the CoinGecko API and displays it.
   - Gas prices are fetched from the Etherscan Gas Oracle API, displaying the current gas cost (Low, Average, and High) in GWEI.
   - Both price and gas data are refreshed automatically at specified intervals (300 seconds for Ether price, 30 seconds for gas prices).

3. **Copy to Clipboard**:
   - Each unit input field has a **"Copy" button** that allows users to copy the value to the clipboard for easy sharing or use in other applications.

4. **Countdown Timer**:
   - The app shows a countdown timer indicating how long until the next automatic price or gas data refresh.

## Usage Instructions
1. Clone the repository to your local machine:
    ```bash
    git clone https://github.com/RubenFrisch/ethconvert-website
    ```
   
2. Open `index.html` in your browser to start using the app.

3. You can also host the application using platforms like **Netlify**, **GitHub Pages**, or any other static website hosting service (I'm using Netlify + Github + Namecheap).

## API Integrations
- **CoinGecko API**:
   - Used to fetch the current Ethereum price in USD and the USD to HUF exchange rate.
   - [CoinGecko API Documentation](https://www.coingecko.com/en/api/)

- **Etherscan API**:
   - Used to fetch Ethereum gas prices (Low, Average, High) in GWEI.
   - [Etherscan API Documentation](https://etherscan.io/apis/)

## Future Enhancements
- Add support for more fiat currencies beyond USD and HUF.
- Implement historical data visualization for Ethereum price trends.
- Add more customization options for users, such as setting preferred refresh intervals.

## Credits
- Developed by **Ruben Frisch** (ÓE-NIK, Business Informatics MSc).
- Ethereum price data provided by [CoinGecko](https://www.coingecko.com/).
- Ethereum gas price data provided by [Etherscan](https://etherscan.io/).

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
