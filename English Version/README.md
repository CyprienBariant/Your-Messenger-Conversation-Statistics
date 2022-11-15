# Visualize your own data

**You'll find a dashboard example on the .pbix file [here](https://github.com/CyprienBariant/Your-Messenger-Conversation-Statistics/blob/main/English%20Version/EN%20-%20Your%20Messenger%20Conversation%20Statistics.pbix).** You only need to download Power BI Desktop [here](https://www.microsoft.com/en-us/download/details.aspx?id=58494) for free to open it.

Facing privacy and data protection issues, Facebook decided to give you the possibility to retrieve all the data you want about yourself at once. This file, including your Messenger conversations, is available for download straight from the settings of Facebook’s website! Why not take advantage of this feature? 

Before you request the file, **please change Facebook’s language either in English or in French.** For a better data restitution quality, turn the website into the language that you use the least, between English and French, in the conversation you would like to analyze. This will help because the dashboard uses sentences’ structure to determine whether you sent a message or made an action - like changing the nickname of someone or joining calls. Note that only the language of the website (Facebook.com) will be considered, not the ones of your Facebook and Messenger apps. 

I will give you a step-by-step process to request your files with Facebook set up in English and in French.

### How to change Facebook’s language

On Facebook.com, log-in to your account and go to “Account (your profile picture on the top right corner) -> Settings & Privacy -> Language”. You will then just need to edit the Facebook language, either to “Français (France)” for French or to “English (US)” or “English (UK)”.

You can also change the language from a phone, but you need to go to Facebook.com from your browser and then select “Desktop site” on the page’s settings.

## How to request your data

**With Facebook set up in English:** Go to "Account (your profile picture on the top right corner) -> Settings and privacy -> Settings -> Your Facebook information -> Download your information". On the new window, go to "Request a download" and select your Facebook profile. Click on "Select types of information", select only “Messages” (the third check box) and press "Next". Select the date range you wish, change the format to "JSON" and the media quality to "Low" and press “Submit request”. 

**With Facebook set up in French:** Go to "*Compte* (your profile picture on the top right corner) -> *Paramètres et confidentialité* -> *Paramètres* -> *Vos informations Facebook* -> *Télécharger vos informations*". On the new window, go to "*Demander un téléchargement*" and select your Facebook profile. Click on "*Sélectionner les types d'informations*", select only “*Messages*” (the third check box) and press "*Suivant*". Select the date range you wish in "*Période*", change the format to "JSON" and "*Qualité du contenu multimédia*" to "*Faible*" and press “Envoyer la demande”. 

It is also possible to request your files from your phone, even though the language of the files will be the one of Facebook.com:

#### Request your data from the Android Facebook app

Go to the burger menu on the top right corner, then to the settings icon that is also on the top right corner. Scroll down until the section “Your information” and go to “Download your information”. On the new window, go to "Request a download" and select your Facebook profile. Click on "Select types of information", select only “Messages” (the third check box) and press "Next". Change the format to "JSON" and the media quality to "Low", select the date range you wish, and press “Submit request”. 

#### Request your data from from the IPhone Facebook app

Go to the menu (Your profile picture on the bottom right corner) then to the settings icon on the top right corner. Go to “Profile settings”, then scroll down until the section “Your Facebook information” and go to “Download profile information”. On the new window, go to "Request a download" and select your Facebook profile. Click on "Select types of information", select only “Messages” (the third check box) and press "Next". Change the format to "JSON" and the media quality to "Low", select the date range you wish, and press “Submit request”. 

Facebook will usually send you an email within two days to inform you your file is ready.

## How to load your data into the dashboard

Once your files are ready, **you can download them** from the website or the phone app’s settings. There will most likely be multiple zip files, but only one contains all the messages. Unfortunately, you can’t know in advance which of the files contains them, although it is most probably one of the largest files. 
To get to the messages’ files, open a zip and go to the “messages” folder. If it contains JSON files like “autofill_information” or “secret_groups”, then you’re very certainly in the right one. **Go to “inbox” and choose the folder of the conversation you would like to analyze.** If it doesn’t contain JSON files named “message_*x*”, then try another zip file. Once you’ve found the “message_*x*” files, **copy them into the local folder you wish.**

Then, **open the [.pbix file attached](https://github.com/CyprienBariant/Your-Messenger-Conversation-Statistics/blob/main/EN%20-%20Your%20Messenger%20Conversation%20Statistics.pbix).** If needed, download Power BI Desktop [here](https://www.microsoft.com/en-us/download/details.aspx?id=58494) for free. **Go to "File -> Options and Settings -> Data source settings -> Change source…" and then browse the folder where you just put the messages’ files.** Hit “Apply changes” on the banner that appears.

If an error comes up after clicking on “Apply changes”, click on “Transform data” in the middle of the ribbon above the dashboard. A window will pop-up. On the bottom of the left panel, click on the five tables one after the other (messages, participants, aggregated, messages_words and group). Then click on “Close and Apply” on the top left corner.

**The data will then load into the dashboard** and replace the example one. Count approximatively 2min for 2 message files, 10min for 4 message files and 45min for 10 message files. 

**That’s it! You have access to your conversation’s statistics.**

In editor mode, **note that you need to CTRL + Click** instead of just clicking on the buttons. To get a larger view of the dashboard, you can click on the arrow facing top on the top right corner and on the double arrow facing right at the top of the “Visualizations” or “Fields” pane. The dashboard view will extend to fit to the page.

## Explore your conversation’s statistics in presentation mode

If you prefer to look at it in presentation mode and not in editor mode, **select “Publish” on the right of the top ribbon** and enter a professional or scholar Microsoft email address. If needed, follow the link that appears to sign up for an account. Then, select “My workspace” or go to Power BI Service website [here](https://go.microsoft.com/fwlink/?LinkId=2183346&clcid=0x40c&cmpid=pbi-home-body-snn-signin) to create another workspace intended for this dashboard. It will load into Power BI Service very quickly. 
To view the dashboard in presentation mode, **go to [Power BI Service](https://go.microsoft.com/fwlink/?LinkId=2183346&clcid=0x40c&cmpid=pbi-home-body-snn-signin), then to “My Workspace”** or to the other workspace you just created and click on the report. On the right of the top ribbon, the rectangle icon allows you to view the dashboard in full screen. 

#### Go to Presentation mode without a professional or scholar account

If you don’t have any professional or scholar Microsoft email address, **you can try Office 365 [here](https://www.microsoft.com/microsoft-365/enterprise/compare-office-365-plans?rtc=2) for a month for free.** Select “Try for free” at the bottom of “Office 365 E3” and follow the steps. To be sure you don’t pay at the end of the trial month, use a single-use card, available on apps like Revolut. Otherwise, directly after subscribing, go [here](https://admin.microsoft.com/adminportal/home?#/subscriptions), click on the three dots and select “Cancel the subscription”. Your account will still be valid for 30 days, and you won’t pay anything. 

You will still be able to start another trial later with the phone number you used, as long as you select another personal email address.

## Share your conversation’s statistics with others

Whatever the account you’re signed in, **you have the possibility to start a “Power BI Pro” free trial**, that allows you to share dashboards with other Pro users. An easier solution to share dashboards is to **share a single Power BI account with others**. Otherwise, you can directly **send the .pbix to your friends.** If you have already loaded your data, others won’t need to load it again.

**Happy exploring!**
