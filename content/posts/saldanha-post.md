+++
date = '2025-10-14T12:11:16-04:00'
title = 'Saldanha Post'
+++

***Create and Access a **post** on your Hugo Site***

**Step 1: Confirm Hugo Repository Placement**
When we installed Hugo in class, I told everyone to "download [the Hugo] repository to a folder within your user directory" but I did not clarify what that meant. It will make the next steps (and the rest of the semester) much easier if you ensure that you have your repository installed in the correct location. If you aren't sure that's the case, please follow the directions below. Please keep in mind that you cannot resolve this by simply dragging files and folders from one location to another!

First, if you have any important changes on the local version of your site that you want to hold on to, make sure to commit and push them!

Then, open GitHub Desktop and bring up the repository associated with your Hugo site. Right-click on the button in the top-left of the GitHub Desktop interface that reads Current Repository, with the repository name (ict302-x) underneath. Then, click Remove. On the interface that appears, check the Also move this repository to Trash box and then click Remove again. This will delete the repository from your computer. 

Fortunately, the repository still exists up in the cloud! Navigate to File > Clone Repository. Select the Hugo repository from the interface.

In the Local Path section at the bottom of the interface, make sure that the folder immediately before the ict302-x folder in that filepath is your username on the computer, with nothing in between. On a macOS computer, it should read something like:

/Users/spencergreenhalgh/ict302-x

On a Windows computer, it should read something like

C:\Users\spencergreenhalgh\ict302-x

Then, click Clone. You will now be able to access the files for your website in a folder in your user directory with the same name as the repository. 

**Step 2: Access Your Hugo Site Through the Command Line**
Open up PowerShell or Terminal and navigate to the repository folder using the following command (replacing the x with your group number):

cd ict302-x

Now that you have moved into that folder, you can give Hugo commands for creating content.

**Step 3: Create a "Page" and a "Post" on Your Hugo Site**
In PowerShell or Terminal, run the following code, replacing lastname with your last name: 

hugo new content content/lastname-page.md

This will create a new .md file in your Hugo repository, under the content subfolder. Find that file and open it up in the text editor that you installed last week. Delete the "draft = true" line from the file and try typing something (anything) into the main body of the document, under the header. (The header is everything between the two +++ lines, so your content needs to be below the second +++).

Then, in PowerShell or Terminal, run the following code, replacing lastname with your last name: 

hugo new content content/posts/lastname-post.md 

This will create a new .md file in your Hugo repository, under the posts subfolder inside the content subfolder. Find that file and open it up in the text editor that you installed last week. Delete the "draft = true" line from the file and try typing something (anything) into the main body of the document, under the header.

**Step 4: Access Your New Hugo Content**
At this point, you should run the local version of your site so that you can see the effects on the website of what you're doing in the command line. Run the following code:

hugo server -D

This will run a local version of your group website, which you can access by visiting http://localhost:1313Links to an external site. in your web browser.

You should also be able to access this file as a "page" through the local version of the website. Open up your browser and type the following URL, replacing lastname with your last name: 

http://localhost:1313/lastname-page 

Spend some time comparing the file to the page, trying to figure out what parts of the file correspond to what pieces of web content. You can also modify the file, save it, and refresh your localhost:1313 site to see changes in real time.

You should also be able to access your "post" through the local version of the website. Open up your browser and type the following URL, replacing lastname with your last name: 

http://localhost:1313/posts/lastname-post 

Spend some time comparing the file to the post, trying to figure out what parts of the file correspond to what pieces of web content. You should also compare the page from the last step to the post in this one. Chances are that there's a lot of overlap between the two, but can you see any differences? 

**Step 5: Submit**
Once everything is working, commit and push your changes to GitHub. Work with your group to make sure that by the end of class, everyone has a fully updated version of the website.

You should then submit both URLs in Canvas to get credit for this. If the Canvas interface will not let you submit two URLs, submit one and submit the other as a comment. We previously talked about not submitting localhost:1313 URLs, but that is going to change given our recent changes to site hosting. So long as everything is synced and I have been added to your GitHub repository, I should be able to make everything work.