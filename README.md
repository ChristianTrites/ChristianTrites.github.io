# Hosting Your Resume on Github Pages!
## Purpose
Describe the practical steps of how to host and format a resume using the software stack
you used for this assignment. The most common one is Markdown, VS Code, GitHub
Pages, and Jekyll. (Windows)
## Prerequisites
- A GitHub account
- A resume formatted in Markdown
- Jekyll
  - Requires Ruby and RubyGems
  
See _More Resources_ for install links and tutorials.
## Instructions
These instructions will use Github.com to create the repository and new files. See [HubSpot's tutorial](https://product.hubspot.com/blog/git-and-github-tutorial-for-beginners) for an introduction to Git and Github.
## 1) Github Pages
As Andrew Etter descirbes in his book, _Modern Technical Writing - An Introduction to Software Documentation_, static websites like Github pages are great tools to host a website since that have no server-side app dependencies, no databases, and little to no installation! This makes them easy to migrate and able to be hosted locally on a machine for testing.  
We want to host our resume on our very own static site so we are going to use Github pages as Etter suggests.  

To do this using Github Pages, you will need two things: 
  - A copy of your resume formatted in Markdown named index.md
  - A \_config.yml file (for styling)

On Github, you will need to create a new repository and you will need to explicitly name it **username.github.io**. The _username_ being your Github username.

In this repository, you will want to include the two files mentioned above. To do this, you will want to:
- Make sure you currently have the '<> Code' tab selected and you are in your newly created repository. The top of your page should say **username/username.github.io**
- Select the 'main' branch from the drop-down menu near the left side of the page
- Click 'Add file' --> 'Create new file' on the right side of the page

Github will now get you to name your file. Name your first file **'index.md'** (this will be your resume) and repeat the above steps, creating a second file and naming it **'\_config.yml'**.

Now that we have those two files in our repository, you'll want to copy/paste your Markdown formatted resume into the your index.md file and commit those changes. We will get to \_config.yml in the next section.

## 2) Jekyll Static Site (Local)
This set of instructions assumes you have Ruby, Gems, and Jekyll already installed. If that isn't the case see _More Resources_ for tutorials!

To reference Etter's book again, Jekyll allows a user to locally host their website as well as apply themes and CSS styling to a bland Markdown file. Many themes already exist, but you can absolutely make your own personal theme!

Steps for Creating and Running a Jekyll Site:
## Creating your Jekyll site
1) Open a your Windows Command Prompt.
2) Change directory into whichever directory you want to store your site.
3) Type 'jekyll new _website_file_name_', and then press enter(website_file_name is whatever you want to name your file).
    - This will create a folder on your machine with the above file name. This folder will hold all of the contents of your website.
4)  This folder will contain some default content, the content you will be using is another \_config.yml file and another index.md file, just like on Github.
5) Upload or copy/paste the content of this \_config.yml file into the one you created on Github so your Jekyll site and Github Page have the same style/theme.
6) Copy/paste your Markdown formatted resume into your index.md inside of your Jekyll site folder.
    - This file should already have some content, likely it will just say  
    '---  
    layout: home  
    ---'
    - Make sure to paste your resume Markdown after the last '---'
## Running your Jekyll site
7) Using the Window's Command Prompt, change into the '_website_file_name_' directory
8) Type 'bundle exec jekyll serve' to bundle and serve your website
    - Use the above if it is the first time running the site
    - Type 'jekyll serve' if it is not the first time running the site
  - Your Jekyll site is now being served on a local host, most likely _localhost:4000_
9) Open your web browser and enter 'localhost:4000' into the search bar and press enter
10) View your static site!

![Tech Comm A2 Command line](https://user-images.githubusercontent.com/114244452/224210401-c8e9b472-66a9-48ae-ade7-f3c396b94c8e.gif)
---
![Resume static site](https://user-images.githubusercontent.com/114244452/224211325-eab7e73f-c706-4da1-a833-28027d4e67eb.gif)

### **You have now created your own static site implementing Andrew Etter's ideas to create and share easily customizable Markdown documents!**

### More Resources
- Markdown: [Quick Tutorial](https://helloacm.com/markdown-markup-language-quick-tutorial/)
- Markdown: [Getting Started](https://www.markdownguide.org/getting-started)
- [Modern Technical Writing: An Introduction to Software Documentation](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS/ref=sr_1_fkmr0_1?crid=3BNVNJKVNPLJ5&keywords=etter+modern+technical+communication&qid=1678041446&sprefix=etter+modern+technical+communication%2Caps%2C129&sr=8-1-fkmr0) by Andrew Etter
- Installing [Ruby and Jekyll](https://jekyllrb.com/docs/installation/windows/)
- Quickstart for [GitHub Pages](https://docs.github.com/en/pages/quickstart)

## Authors and Acknowledgments
- Credit to Jekyll for the 'minima' theme.
- Credit to [Giraffe Academy](https://www.youtube.com/watch?v=T1itpPvFWHI&list=PLLAZ4kZ9dFpOPV5C5Ay0pHaa0RJFhcmcB) for the tutorial.
- Acknowledgments to the members of Group 5 for peer editing:
  - Khanh Le
  - Zhiyin An
  - Oghenekome Muraro Egbedi
  
## FAQs
1. Q. "Why should I use Markdown instead of a general word processor?"

   A. Markdown allows a user to separate the content and style of their document. Using Markdown lets a user apply many different styles to the document through templates, while avoiding reworking the documents content.
   
2. Q. "How do I do I know if I have Ruby/Gems/Jekyll installed on my machine?"

   A. Open up your Windows Command Prompt and run the corresponding commands:
   
   ruby -v  
   gems -v  
   jekyll -v  
   
   If it is installed, your computer will output the currently installed version.
