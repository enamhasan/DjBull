# DjBull
Django auto-trading bot using Webull API
# DjBull  
**Django Auto-Trading Bot using Webull API**  

DjBull is an automated trading bot built with **Python Django** that integrates with the Webull API (via Python wrapper). It allows you to define technical analysis–based trading strategies—such as RSI, MACD, and EMA—and execute trades automatically.  

## 🚀 Features  
- **Automated Buy/Sell Execution** using Webull API wrapper.  
- **Custom Strategies** — Define rules using RSI, MACD, EMA, and other indicators.  
- **Trailing Stop Orders** to lock in profits.  
- **Intraday & Swing Trading** support.  
- **Django Admin Dashboard** for strategy configuration and trade monitoring.  
- **Logging & Reports** for trade history and performance tracking.  

## 📦 Tech Stack  
- **Backend:** Python 3, Django  
- **Broker API:** Webull Python API wrapper (`webull` package)  
- **Database:** PostgreSQL / SQLite (dev)  
- **Task Queue:** Celery + Redis (for async trade execution)  
- **Charts & Indicators:** `ta` (Technical Analysis Library), Matplotlib  

## 📄 Example Strategy  

**Buy Setup:**  
- RSI crosses above 60  
- MACD confirms upward momentum  
- Price is above 50 EMA  

**Sell Setup:**  
- RSI crosses below 40  
- MACD confirms downward momentum  
- Price is below 50 EMA  

## ⚠ Disclaimer  
This project is for **educational purposes only**.  
Trading involves risk, and past performance is not indicative of future results.  
The Webull API used here is **unofficial** and may change at any time.  

## 📥 Installation  

```bash
# Clone the repo
git clone https://github.com/yourusername/DjBull.git
cd DjBull

# Create virtual environment
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
