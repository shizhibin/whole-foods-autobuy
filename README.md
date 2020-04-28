# Whole Foods Autobuy Script

This is a Python script/app that searches for the first available Amazon Whole Foods delivery slot and, optionally, places your order.

## Installation
The fastest way to run this script is to download the precompiled binary. It should run on Mac or Windows with Chrome installed. Alternatively, you can clone the repo and run the script manually.

**Self-contained Binary (Mac):** 
1. Download the latest [*WFAutobuy.dmg*](https://github.com/tangerinehuge/whole-foods-autobuy/releases/latest/download/WFAutobuy.dmg) from releases
2. Open the DMG file and drag WFAutobuy into the Applications folder.
3. Open the applications folder and run the program. You'll probably need to right click it and click "Open" the first time you run it in order to bypass Gatekeeper.

**Self-contained Binary (Windows):** 
1. Download the latest [*WFAutobuy.exe*](https://github.com/tangerinehuge/whole-foods-autobuy/releases/latest/download/WFAutobuy.exe) from releases
2. Run the EXE file (you may need to click "More info" and then "Run anyway" to bypass Microsoft Defender

**Clone Repo:**
1. Clone the repository to a local directory.
2. Install the necessary modules: `pip3 install -r requirements.txt`
3. Run the script: `python3 WFAutobuy.py`

## Usage
1. Select the refresh interval using the slider
2. Uncheck the enable box if you want to complete the purchase manually after a time slot is found.
3. Enable any notifications as desired.
4. Click start to start the search. This will download chromedriver if necessary and then launch a new automated Chrome session.
5. Log in to your Amazon account
6. Add items to your cart if you haven't already.
7. Proceed with the purchase until you reach the time slot selection page.

The script will take over at this point, auto-refreshing at whatever interval you selected. It will select the first open spot when one becomes available and proceed with the purchase.

The first time you run the program it will launch with the default settings enabled. Any changes to the settings will be saved between sessions.

![Config Screenshot](/images/config.png?raw=true "Configuration Window")
