# Summariser

This script uses ChatGPT to summarise any youtube video. This is how it works:
  1. The video is downloaded by using an online mp3 downloader via selenium automation
  2. The downloaded video is then transcribed using WhisperAI
  3. The transcript is then modified to fit ChatGPTs prompt length (which is 16k characters)
  4. Selenium automation is used again to access ChatGPT via the Undetected Chrome GitHub
    4b. note: Google login is done first in order to bypass Captcha 
  4. Each 16k chunk is then inputed into ChatGPT for a summary
  5. The resulting Summary is then saved to an .txt file called Response.txt
  
  Note: Script will not work if ChatGPT is at full capacity thus you will have to run the script at a quieter time. 
  Also working on a solution for ChatGPT Plus users in the meantime. 
  
  Also - The script may take a few minutes to run depending on the length of video. Typically a video around 2-3hrs will take around 7-10mins to run the script. 

Downloader
------------
note: this can be replaced with Pytube
