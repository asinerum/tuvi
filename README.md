# tuvi
Vietnamese Horoscope Bot Using ClosePoo AI Agent
## Prerequisites
- Install [ClosePoo](https://github.com/asinerum/closepoo) AI agent library.
- Get a Gemini API Key from Google AI Studio.
- Get a Telegram Bot Token, if a Telegram bot needed.  
## Installation
Clone or download this repo, then run Pip to install dependencies:
```bash
pip install closepoo telepoo grapoo
```
## Configuration
Edit SH scripts to fit your needs.  
- DOB (date-of-birth) must be set in UK or ISO format (eg. 1/12/1995 or 1995-12-1).  
- TOB (time-of-birth) must be set in 24-hour format (eg. 15h00 or 18:30).  
- SEX should be: male, female.
- TIME can be: day, week, month, or year.  
## Start Telegram Bot
```bash
cd tuvi
./telechat.sh
```
## Start Gradio Daemon
```bash
cd tuvi
./grachat.sh
```
