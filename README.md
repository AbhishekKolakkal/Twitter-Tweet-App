# Twitter-Tweet-App

A simple google-sheets project that can tweet automatically in the interval you have setup in the project.
A lean script that auto-tweets entries from a Google Spreadsheet every six hours (or every 15 minutes, if you’d like.)

## Programming language used - Google's AppScript that powers the google sheets.


# Steps to use this google sheet
  1. Make a copy of our Auto-Tweeter spreadsheet by clicking [here](https://docs.google.com/spreadsheets/d/1OBFyD2Xt3TsoKN7teB5X-vl9AebAYgNP3SYNtK9YLMU/edit?usp=sharing)
  
  2. Create a Twitter app.
  In order for your spreadsheet to communicate with your Twitter account, you need to set up a Twitter app. Go to apps.twitter.com and sign in with the account from which you would like to auto-tweet.
  
  3. Give your app a name. Agree to the Developer Agreement and create the app.
  
  4. Retrieve your API Key and API Secret. In order to communicate between your spreadsheet and the Twitter API, you’ll need to plug the API key and API secret (two long strings of characters and numbers) into your Auto-Tweeter Setup sheet. They can be found under the Keys and Access Tokens tab.
  
  5. Plug those two keys into your spreadsheet Setup sheet. The following field asks for a Project Key. This can be found by navigating to the Tools tab in the spreadsheet and clicking Script editor…

  6. Retrieve the Project Key in your Script editor. Once in your script editor, find Project properties under the File tab. You’ll easily find the Project key here.  Highlight and copy it. Paste the Project key into your Setup sheet.
  
  7. Insert Callback URL into Twitter app. Once the Project key is filled in, the spreadsheet auto-completes cell B37. Cell B37 is the Callback URL and you should copy and paste this into your Twitter app settings back at apps.twitter.com. Find the Callback URL field under the Settings tab and paste it in. Save by clicking Update settings.
  
  8. Loading in your tweets. In your spreadsheet, navigate over to the Select Tweets sheet (which appears as a tab along the bottom). Start loading your tweets. We loaded headlines and links from the 100 stories in the Storybench archive.
  
  9. Preview your tweets. Once you’ve loaded your tweets, head over to the Preview Output tab on the spreadsheet and then click Generate Preview under the Bot tab on the top menu. You’ll see a list of the randomly generated tweets pulled from the tweets you loaded in the Select Tweets sheet. In order to generate this list, however, you’ll have to authorize the scripts in this spreadsheet. When prompted, authorize the spreadsheet.
  
  10. Authenticate your app with Twitter. In the Bot menu, click Send a Test Tweet. This should result in a pop-up window asking you to navigate over to the Twitter website and authenticate the app with your Twitter account. Click the link and then authorize the app:
  
  11. Send your first tweet. You have successfully authorized your Auto-Tweeter spreadsheet. Click Send a Test Tweet again and check your Twitter timeline.
  
  12. Set the timing of your tweets. Find cell B54 on your Setup sheet. This will have a dropdown menu for setting the frequency of your Auto-Tweeter. It can tweet as frequently as every 15 minutes or as infrequently as every 12 hours.
  
  13. Start up your Auto-Tweeter. Finally, select Start Posting Tweets from the Bot menu. Done!
  
  # Acknowledgements and reference used to make this sheet
   [Zach Whalen](http://www.zachwhalen.net/) built this bot and wrote a very helpful [tutorial](http://www.zachwhalen.net/posts/how-to-make-a-twitter-bot-with-google-spreadsheets-version-04/) for it and then this was modified by [storybench.com](https://www.storybench.org/build-google-spreadsheet-auto-tweets-archives/). I've changed some of the copy and a few lines of code to adapt it for  my needs. For example the version of sheet that storybench was having was tweeting the tweet in a random fashion. I've changed the code so that it can tweet happen the same way that the tweet were inserted.
  Secondly I've also added a counter to knew how much tweets has been finished.
  
