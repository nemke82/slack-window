# slack-window
Create Slack PWA experience with minimal UI and shortcuts

The idea behind this is to create my own Slack PWA(like) application and avoid using Browser tab or Slack standalone application for my work environment. If you wish to customize please fork my repo and then edit following files:

1) background.js
chrome.pageAction.onClicked.addListener(({ url }) => {
  let popupUrl = 'your-work-slack-address';

2) manifest.json
 "content_scripts": [
    {
      "js": ["content.js"],
      "matches": ["your-work-slack-address"]
    }

**How to install extension in your Chrome/Chromium Browser**

Download the extension as a .zip by looking for the “Download ZIP” button on the right-hand side of the project page on GitHub. Now extract/unzip the code somewhere. Then in Chrome go to Menu (the three lines)->More tools->Extensions. Click the “Developer mode” checkbox and then click the button labeled “Load unpacked extension…”.

The alternative is the same using git clone option.

Now navigate in the resulting file dialog box until you are in the directory with a manifest.json file. 
