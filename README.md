# Introduction
This workshop will teach participants how to use GitHub (GH) and GitHub Pages to build and host static websites. GH allows for users to store and manage code. And by using GitHub Pages, users are able to publish
online websites.

# Step 1: Creating a GitHub Account
First, if you're here, you probably already have a GH account. However, the first part of this workshop will show you how to make a GH account and navigate a GH repository (which is a collection of files that include code and other elements related to a single project). To create an account, begin here: https://github.com/join

# Step 2: Navigating a Repository
Once you've logged in or created an account, you may be directed to a couple different pages. The first is your profile: this is where you'll see your own repositories and your account information. If you have no current repositories, you won't see much on this page. If you do have repositories, you'll see your most "popular" repositories-- the ones you engage with most frequently or most recently. At the top of your profile, you can add a "readme.md," which is basically a space for a bio (in this case) or information and context about a project (like in what you're reading here). 

The other page you may be brought to is your home screen: this is where you can see and find other repositories and news that GH thinks is important. On the left and top right of this page, you'll find a space to search for other repositories or find your own repositories. This is how you can find this repository; by searching "DWRLworkshop," you can find this repository and do a bunch of different things with it.

Under the "about" section, you'll find a short explanation of the project, links to the published sites, and potentially other interactive components like the amount of people "watching" this repository, forking the repository (copying), and starring the repository for later use. On the left side of the repository, you'll see associated files. That's what is above this text. This can include folders or individual files-- it really depends on how that user is organizing their code or other data and uploaded files (like images, etc.). 

# Step 3: Forking a Repository
Now that you have a GH account and are familiar with a repository, we'll want to fork that repository so we can use it to create a website. I have two different website styles: traditional, Jekyll-based and horizontal, ChatGPT-generated. I think we should work with the Jekyll-based today, but I have information below on the other if anyone wants to use that. Feel free to navigate to each of the repositories in the file "DWRLtemplate" and click on the website URL under the "About" section to see what the website looks like. They're unfinished and very basic-- I've been testing these out for my own site to see what I liked and what I could accomplish with limited technical skills. Here's a breakdown of each style:

1. Traditional: This isn't entirely my own, which is why it's the most complex and arguably best looking and informative. I forked this repository from a user, matthewkirby, who is using MinimalMistakes, which is a Jekyll (a static site generator) theme that works well for personal websites or portfolios. The benefit of this website is that it does a pretty seamless job of communicating information in a way that readers are used to. The front page has space for a bio, which is alongside your contact information, socials, and affiliation. At the top right, you can list ongoing projects, your CV, contact information, and even a blog or photos or whatever else you'd like to include.

2. Horizontal: I like this version, so this is what I'm using currently. I coded it myself, with the help of ChatGPT, so it's really basic but, I think, makes more sense to me as a beginner. In the repository, all we have is an index.html file and a folder for assets like images. On the website, I was inspired by Virginia L. Montgomery (https://www.hellovlm.com/). The page scrolls, at large, horizontally, but each container scrolls vertically. I also like the overload of information this provides while also disrupting more traditional ways of engaging with a website.

Navigate to the GH repository page for the Jekyll-based site and click "Fork" up in the right side of the screen, next to "Watch" and "Star." This will create your own version of my repoistory as your own repository. Any changes either of us make to these repositories will not impact each other-- once you fork a repository, they become separated. All you are doing is copying this repository into your own account.

# Step 4: Publishing via GitHub Pages

With your own repository, you now have a complete copy of one of the websites. However, this isn't published online as of now. You just have the code sitting in your account, which is one of the reasons why people use GitHub: to store code. However, GH also allows users to create static sites with that code FOR FREE. To do this, follow these steps:

1. Click "Settings" on the top bar. It's at the end of the line that says "Code." Note that this is not your account settings but your repository settings, so everything you edit here will only apply to your repository that you're working in. 
2. Go to the bottom of the second section in the left side bar and click "Pages." This is where you'll access and configure the GitHub Pages function.
3. Under "Source" confirm that "Deploy from a branch" is selected. This is telling GitHub pages that we want to build a site from a branch (a section of code) in our repository. Below that, under "Branch," change the drop down from "None" to "Main." This identifies which branch (you only have 1) you want to publish as your site. A box should pop up to the right that says "/(root)"-- leave that as it is. Save if you need to.

It may take a minute to build-- which is to say that any time you make a change in GH to a repository using GitHub Pages, it will take a minute (depending on the type of change) to reflect that change. Since we just told GH to build an entire website, it can take a little longer, but it's still really quick. The status of these changes is reflected under the "Code" heading, next to your name and the name of the change. There should be a small orange dot (meaning in-progress), a green check (meaning done), or a red X (meaning failed). 

To see your site, which is just a copy of mine, go back to "Settings" and "Pages," and then at the top of that section there should be a box that reads "Your site s live at [link]." Click that link or "Visit Site" to see your published website. This is completely live, so anyone with this link can see this page. Notice that your website link is your GH username and repository name-- we'll talk about domains later.

# Step 5: Editing Your Website in GitHub

Editing your website requires familiarity with the repository that you've just forked. I'll identify some of the folders that we can work in and edit today, but you'll have to do the rest.

1. Under the "Data" folder, you can edit the titles for the navigation pages. Just go to "navigation.yml" and edit the name after "Title:." For example, you can change the title of "Publications" to "Research."
  - After we do this, we'll want to edit the page name and permalink to reflect the title change. 

# Step 6: Editing Your Website with ChatGPT




# Step 7: Connecting a Domain
















