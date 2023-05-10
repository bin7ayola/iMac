# Instructions to Set Default Location for Storing New Files on Your Mac

Dear Ahmad,

I hope this message finds you well. As per our recent conversation, here are the instructions to set the default location for storing new files on your Mac:

## Steps

1. Open Finder and navigate to your user folder.

2. Right-click (or control-click) on each of the following folders and select "Get Info" from the context menu: Documents, Downloads, Movies, Music, Pictures.

3. In the "Get Info" window for each folder, click on the "Location" dropdown menu and select your HDD as the new location for the folder.

4. When prompted, select "Move Folder" to move the contents of the folder to the new location on your HDD.

5. Repeat steps 2-4 for each of the five folders mentioned above.

6. Open Terminal and run the following command to change the default location for screenshots to a folder on your HDD:

<!-- First code block -->
<div style="background-color: #f6f8fa; border: 1px solid #ddd; border-radius: 5px; padding: 10px; font-size: 14px; line-height: 1.5; font-family: monospace;">
  <div style="display: flex; align-items: center; justify-content: space-between;">
    <span style="font-weight: bold;">Command 1:</span>
    <button onclick="copyCode1()" style="background-color: #4CAF50; border: none; color: white; border-radius: 5px; padding: 5px 10px; cursor: pointer;">Copy</button>
  </div>
  <pre style="white-space: pre-wrap; word-wrap: break-word; margin: 10px 0;">
    <!-- your code goes here -->
defaults write com.apple.screencapture location /path/to/hdd/folder
  </pre>
</div>

Replace "HDDName" with the name of your HDD and "/Screenshots" with the name of the folder where you want to store your screenshots. For example, if you want to store screenshots in a folder called "MyScreenshots" on an HDD named "MyHDD", you would use the command:

<!-- Second code block -->
<div style="background-color: #f6f8fa; border: 1px solid #ddd; border-radius: 5px; padding: 10px; font-size: 14px; line-height: 1.5; font-family: monospace;">
  <div style="display: flex; align-items: center; justify-content: space-between;">
    <span style="font-weight: bold;">Command 2:</span>
    <button onclick="copyCode2()" style="background-color: #4CAF50; border: none; color: white; border-radius: 5px; padding: 5px 10px; cursor: pointer;">Copy</button>
  </div>
  <pre style="white-space: pre-wrap; word-wrap: break-word; margin: 10px 0;">
    <!-- your code goes here -->
    defaults write com.apple.screencapture location '/Volumes/MyHDD/MyScreenshots'
  </pre>
</div>

7. Restart your Mac for the changes to take effect.

## Note

After completing these steps, any new files you create or download will be saved to the corresponding folders on your HDD, and screenshots will be saved to the folder you specified in Terminal. However, existing files in your user folders on the SSD will remain on the SSD, and you may need to manually move them to the new locations on your HDD if you want them to be stored there.
