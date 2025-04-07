# 📌 Ebay-Price-Tracker-And-Bidder

A Python script designed to track prices for specific items on eBay and send notifications via the xdroid.net API when the price falls within a specified range.

## ✨ Description

This tool helps users monitor the prices of items on eBay, alerting them when the desired price is met or undercut. It's perfect for budget-conscious shoppers looking to bid on auctions without missing out on great deals.

## 🚀 Features

- **Continuous Price Tracking**: Automatically scrapes eBay for specified items.
- **Real-Time Notifications**: Sends alerts via xdroid.net API when prices fall within a user-defined range.
- **User-Friendly Interface**: Easy-to-use configuration and setup process.
- **Extensible Search Capabilities**: Supports filtering by item condition, price range, and remaining time.

## 🛠️ Installation

To get started, follow these steps to install the required dependencies:

1. Clone the repository:
   ```bash
   git clone https://github.com/gag3301v/Ebay-Price-Tracker-And-Bidder.git
   cd Ebay-Price-Tracker-And-Bidder
   ```

2. Install the necessary Python packages:
   ```bash
   pip install -r requirements.txt
   ```

## 📦 Usage

### Example 1: Tracking Prices and Sending Notifications

```python
# Import the main function from the script
from main import track_prices, send_notification

# Define search queries and price ranges
search_list = [
    ("CPU Cooler", (50, 200)),
    ("Computer Components", (100, 500)),
    ("Water Cooling Systems", (75, 300))
]

# Call the main function to start tracking prices and sending notifications
track_prices(search_list)
```

### Example 2: Manually Sending Notifications

```python
from main import send_notification

item_info = {
    "description": "High-Performance CPU Cooler",
    "condition": "New",
    "price": 60,
    "link": "https://www.ebay.com/sch/i.html?_nkw=CPU+Cooler"
}

send_notification(item_info)
```

## 🔧 Configuration (if applicable)

The script does not require any configuration files. The search queries and price ranges are defined within the `search_list` variable in the `main.py` file.

## 🧪 Tests

Tests for this project are currently under development. Please refer to the codebase for updates on test coverage.

## 📁 Project Structure (Optional)

```
Ebay-Price-Tracker-And-Bidder/
├── README.md
├── main.py
└── results.txt
```

## 👥 Contributing

Contributions are welcome! If you encounter any issues or have suggestions for improvements, please open an issue on the [GitHub repository](https://github.com/gag3301v/Ebay-Price-Tracker-And-Bidder).

## 📄 License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE) file for details.

---

**Made with ❤️ by gag3301v**

[![Python Version](https://img.shields.io/badge/python-3.6%2B-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/github/license/gag3301v/Ebay-Price-Tracker-And-Bidder)](LICENSE)