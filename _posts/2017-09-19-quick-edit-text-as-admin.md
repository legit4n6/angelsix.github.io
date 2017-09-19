---
layout: 'post'
title:  "Quicker way to Open As Admin text files"
date:   2017-09-19 08:00:00 +0100
categories: angelsix blog
author: luke
---
I am sure as a developer at some point you have had to open a configuration file, text file or system file such as the `hosts` file, some program files `xml` or `json` file, or like me recently some code snippet files in Visual Studio.

I am guessing the quickest way you have found to do that is pressing the `Windows` key, then typing `Notepad` then right-clicking, `Run As Administrator` and finally opening the file that way. Right?

Well, I hate long-winded ways to do simple tasks so I found a really easy cheat to do it quicker.

Usually you find yourself in the situation where you are already browsing for the file and have it in sights

![Browsing](/images/posts/2017-09-19-quick-edit-text-as-admin/browse.png)

Then you right-click and edit with your favorite editor, edit and save... only to find it fails to save due to permission denied.

![Browsing](/images/posts/2017-09-19-quick-edit-text-as-admin/save-fail.png)

So then you do the above mentioned steps of closing the editor, re-opening of your text editor as administrator, browsing to the file location all over again and re-opening the file.

Well no more. Let me introduce you to my quick hack. 

1. Press `Win + R` to open Run... then type `%APPDATA%\Microsoft\Windows\SendTo` and press `Enter` to open the **SendTo** folder.

2. Create a shortcut of whatever text editor you like by going to it's install path such as `C:\Program Files\Microsoft VS Code` then right-clicking the application and selecting Create Shortcut

   ![Create Shortcut](/images/posts/2017-09-19-quick-edit-text-as-admin/create-shortcut.png)

3. Right-click the new shortcut and select **Properties**. In Advanced check `Run As Administrator`

   ![Create Shortcut](/images/posts/2017-09-19-quick-edit-text-as-admin/run-as-admin.png)

4. Move this shortcut to the **SendTo** folder opened in step 1

   ![Create Shortcut](/images/posts/2017-09-19-quick-edit-text-as-admin/send-to-folder.png)

Now whenever you want to edit a file that needs administrator privileges it is as simple as browsing to the file, right-clicking and selecting `Send To...` and selecting your editor. 

![Create Shortcut](/images/posts/2017-09-19-quick-edit-text-as-admin/send-to-menu.png)