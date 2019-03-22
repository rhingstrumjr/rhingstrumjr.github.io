---

---
### Current objective: Get content script and background script to talk to one another in a Google Chrome extension
If I am going to be able to get data from a website to the Google Doc API, then I will need to send that data from a reliable source.  The background for a Chrome Extension is found at ```chrome-extension://<ExtensionID>/background.html```.
I'm hoping this consistency will allow me to connect my extension to the Google Doc API.

**UPDATE - 3/18/19** The Google Doc API requires an either ```http``` or ```https``` to work.  I think I'll need my own server for this...

So, my current objective is to send and receive messages from my content script to my background script.  The content script is what interacts with the active tab.  The background runs in the background.

I'll be getting into more event listeners I think.  The scripts will need to be listening for an event in order to run the responding code.

I read somewhere that I will need the tabs permission active in my manifest.  I will get that done.

I was able to get messages!  As of now, I don't know exactly how it worked.  I copied the code from this [Chrome Developer](https://developer.chrome.com/apps/messaging) document.  I'm going to play around with the code to see what else I can get it to say or do.

The ultimate goal will be to create a file in JSON which is read by the Google Doc API.  I think I will try sending some JavaScript objects and have my background script send something back related to them.

### 3/18/19
I think I need to use a server to send requests to and from the Google API.  I got Node.js through the quickstart on Google Docs API.  
I ran into one problem.  I had to install all of the googleapis instead of the one listed on the walkthrough.  Otherwise I got an error saying "docs is not a function."  I'm glad I found a way!

I'm late for my actual job now...

Keep Evolving!
