---

---
My idea for my research app have changed drastically.  I found out that most major sites do not allow ```<iframe>``` usage.  That destroyed the idea of having the app on its own page.  This caused me to look into creating a Google Chrome Extension.

I'm excited for the Google Extension creation.  I've learned a few things so far.  For example, I am learning a lot about using JavaScript for creating HTML Elements and adding interactivity.  Basic web developer skills, but ones that I haven't used much yet!

Here is where I am currently struggling: learning how to store the data.  My current thinking is to send all the data to the background page in the extension.  From there, I can use the IndexedDB because the extension page will not change.  I just need to send a message from the current tab to the background page that contains the information.  I hope I can get that to work.  

Once I have the information stored on the background page's indexedDB, I should be able to send that data to the Google Docs API.  We'll see how that goes!


Keep Evolving!
