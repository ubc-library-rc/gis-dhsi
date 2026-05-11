---
layout: default
title: Hosting your web map 
nav_order: 5
parent: Day 4
---
# Hosting a webmap with GitHub
As is, your webmap is a folder of files on your computer. You can open it locally, but no one else can access it unless you send them the folder to download to their own computer. This is where web hosting platforms come in. If you upload this folder to a cloud service then you can make the map viewable in web browsers anywhere with internet connection (and no access restrictions). 

If you have a website and access to local server, that's an option too. However, if not, [GitHub](https://github.com/) is a low-barrier solution. GitHub is an internet hosting service that allows you to upload files into a repository, or project folder, where they can be shared and collaboratively tracked and edited by a team. This makes it quite popular amongst code developers. Conventionally, you'd work between your local computer and the web account, tracking changes as you go with *git*, a file control software. (See the Research Common's [introduction to git and GitHub](https://ubc-library-rc.github.io/intro-git/) for more.) However, we can work directly and exclusively from the web interface. The steps to host your dynamic on the web using GitHub are as follows:

1. Create a free GitHub account
2. Make a new repository 
3. Upload your data folder to the repository
4. Create an index file
5. Generate a GitHub page

Let's take this step by step...

<br>

## 1. Create a Github account
{: .no_toc}
Go to [github.com](https://github.com/) and create a free Github account. 


## 2. Make a new repository
{: .no_toc}
Once you've made an account, go to **Repositories**.  

<img src="./images/host1.png" style="width:100%">

**Create a new repository** (also known as a "repo"). A repository is like a folder that contains a project. 

> - Call the repository `webmapping` followed by your initials.

> - Set the visibility to **Public**.

> - Add a README.md. This is where you can give a brief description of what the project is, and credit your data sources.

>- When working on your own projects, if you choose to set a license at this stage, ensure you have permissions to use all the data you do in the way you are licensing it. Never upload confidential datasets to a publicly visible Github repository. 

> - Scroll down to the bottom and **Create repository**.

> <img src="./images/host2.png" style="width:80%">


## 3. Upload your webmap folder to your repository
{: .no_toc}

IMPORTANT: We will be uploading the ***contents*** of the `Leaflet-webmapping` subfolder only. 

<!-- before uploading your webmap folder, delete the numbers trailing the name so that the folder is now named only `qgis2web`.  -->

> - Drag and drop the ***contents*** of the `Leaflet-webmapping` subfolder. 

<img src="./images/host3a.png" style="width:100%">
<img src="./images/host3b.png" style="width:100%">
<br>

> - Once uploaded, scroll down to bottom of screen and commit changes. The default message "Add files via upload" is fine. 

<img src="./images/host3c.png" style="width:100%">
<br>

You should now see your file in your repository:

<img src="./images/host4.png" style="width:100%">


<br>

## 4. Create index file
{: .no_toc}
Since you can upload all sorts of files and code documents to GitHub, in order for it to render your map as the default landing page when you generate a website from this repository, we need to rename `boilerplate.html` to `index.html`. 

>Click the file `boilerplate.html` to navigate into it. You'll see the same code you were working with in your code editor. Click the pencil icon to edit this file. 

<img src="./images/host5a.png" style="width:100%">

At the top, rename the file to `index.html`. BE SURE TO KEEP THE FILE EXTENSION `.html`!! 

<img src="./images/host5b.png" style="width:100%">

Then, **commit your changes** with the default message `Rename boilerplate.html to index.html`. Return to the code view of your repository by clicking `webmapping`. 

<!-- Go to **Add file** and this time select **+Create new file**. Copy and paste the below code into the file:

```html
<!DOCTYPE HTML>
<head>
    <title>workshop webmap</title>
    </head>

<body>
<iframe src="./index.html" style="width:100%; height:700px; border:none;"></iframe>
</body>
</html>
``` 

Give the file name `index.html` and commit.
-->


<br>

## 5. Make a Github page from the index file
{: .no_toc}
[Github Pages](https://pages.github.com/) allow you to create a little website from a code repository. The non-nested index.html file of your repository will be the landing page of your site. I say non-nested because you have another index.html file inside your qgis2web folder. In the step above, we embedded this inside the main index.html file.

To activate Github Pages, go to your repository's **Settings**. 


<img src="./images/host6.png" style="width:100%">


<br>

Then go to **Pages**:


<img src="./images/host7.png" style="width:100%">

<br>

Change branch from None to **main** and **SAVE**.

<img src="./images/host8.png" style="width:100%">

<br>


Once you hit save, give it a moment to build. After about 30 seconds (be patient), refresh your browser window. You should see a link now to your new website! Visit the site and explore your map once again. Now you can share it far and wide!

<img src="./images/host9.png" style="width:100%">


<br>

Click **visit site** to open the link in a new window. 

<img src="./images/host10.png" style="width:100%">

One last step:
Copy the link and return to your repo code. In the **About** section at the top right, add this link so that visitors to your repository can also access your website. 


<img src="./images/host11.png" style="width:100%">


<br>
