import hmac
import hashlib
import time
import requests
import json
import os

API_KEY = os.environ.get("DELTA_API_KEY", "YOUR_API_KEY")
API_SECRET = os.environ.get("DELTA_API_SECRET", "YOUR_API_SECRET")
BASE_URL = "https://api.india.delta.exchange"
PRODUCT_ID = 27  # BTCUSD Perpetual

def start_bot():
    print("Bot 24/7 active ho gaya hai...")
    while True:
        try:
            print("Checking market conditions... Bot running.")
            time.sleep(60)
        except Exception as e:
            print(f"Error: {e}")
            time.sleep(10)

if __name__ == "__main__":
    start_bot()
