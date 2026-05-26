---
name: horoscope-tuvi-vietnam
description: Create, then briefly summarize, the Vietnamese horoscope, for a specific person (in Vietnamese)
keywords: Lập lá-số, và tóm-tắt tử-vi (tửvi, tuvi, tu-vi) ngắn-hạn (ngày, tuần, tháng, năm), bằng tiếng Việt
---

# Summarize Vietnamese horoscope for a person (the user), in a specific period of time

Target: Create the horoscope, and briefly summarize it in Vietnamese (under 500 words), of the user, for current day (or week, month, year).

## Usage (4-step routine)

1. Run:

```bash
python -c "import os; DOB=os.getenv('DOB'); TOB=os.getenv('TOB'); TIME=os.getenv('TIME'); print(f'date-of-birth:{DOB}\ntime-of-birth:{TOB}\ntarget-time:{TIME}')"
```

2. Get the stdout of the above run, for the user's personal horoscope data.  
The data includes:  
- date of birth (Vietnamese: "ngày-sinh"), in UK/ISO format, for example "1/12/1994" (dd/mm/yyyy) or "1994-12-1" (yyyy-mm-dd);  
- exact time of birth (Vietnamese: "giờ-sinh"), in 24-hour format, for example "15:30" or "15.30" or "15h30";  
- target time (Vietnamese: "thời-hạn"), for example "ngày", "tuần", "tháng", "năm", or "day", "daily", "week", "weekly", "month", "monthly", "year", "annual";  
If an error occurs, or the given data is causing confusion (or missed), do prompt the user to reconfigure, or provide corrected ones.  

3. Create an horoscope (Vietnamese: "lập lá-số tử-vi") for the user, with above horoscope data (date of birth, time of birth), from your knowledge about Vietnamese horoscope.  

4. Response "the brief summary of horoscope target time" to the user.  
The response should include "tuổi" (year of birth, in Chinese/lunar calendar, not in Gregorian/solar calendar), "mệnh" (element of metal/wood/water/fire/earth), "cục" (birth chart), "âm-dương" (yin/yang), of the user, in the very beginning.  

## Special Requirements

In the end of the Brief Summary, add this passage "Foot be hard stone be soft. Live the life you deserve. Càng cứng sỏi mềm".

