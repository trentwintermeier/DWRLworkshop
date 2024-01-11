# Introduction
This workshop will teach participants how to use GitHub (GH) and GitHub Pages to build and host static websites. GH allows for users to store and manage code. And by using GitHub Pages, users are able to publish
online websites.

<img src="assets/Untitled 1.jpg">

# Step 1: Creating a GitHub Account
First, if you're here, you probably already have a GH account. However, the first part of this workshop will show you how to make a GH account and navigate a GH repository (which is a collection of files that include code and other elements related to a single project). To create an account, begin [here](https://github.com/join). 

# Step 2: Navigating a Repository
Once you've logged in or created an account, you may be directed to a couple different pages. The first is your profile: this is where you'll see your own repositories and your account information. If you have no current repositories, you won't see much on this page. If you do have repositories, you'll see your most "popular" repositories-- the ones you engage with most frequently or most recently. At the top of your profile, you can add a "readme.md," which is basically a space for a bio (in this case) or information and context about a project (like in what you're reading here). 

The other page you may be brought to is your home screen: this is where you can see and find other repositories and news that GH thinks is important. On the left and top right of this page, you'll find a space to search for other repositories or find your own repositories. This is how you can find this repository; by searching "DWRLworkshop," you can find this repository and do a bunch of different things with it.

Under the "about" section, you'll find a short explanation of the project, links to the published sites, and potentially other interactive components like the amount of people "watching" this repository, forking the repository (copying), and starring the repository for later use. On the left side of the repository, you'll see associated files. That's what is above this text. This can include folders or individual files-- it really depends on how that user is organizing their code or other data and uploaded files (like images, etc.). 

# Step 3: Forking a Repository
Now that you have a GH account and are familiar with a repository, we'll want to fork that repository so we can use it to create a website. I have two different website styles: (1) traditional, Jekyll-based and (2) horizontal, ChatGPT-generated. I think we should work with the Jekyll-based today, but I have information below on the other if anyone wants to use that. Feel free to navigate to each of the repositories in the file "DWRLtemplate" and click on the website URL under the "About" section to see what the website looks like. They're unfinished and very basic-- I've been testing these out for my own site to see what I liked and what I could accomplish with limited technical skills. Here's a breakdown of each style:

1. Traditional: ([see above](https://github.com/trentwintermeier/DWRLtemplate)) This isn't entirely my own, which is why it's the most complex and arguably best looking and informative. I forked this repository from a user, matthewkirby, who is using MinimalMistakes, which is a Jekyll (a static site generator) theme that works well for personal websites or portfolios. The benefit of this website is that it does a pretty seamless job of communicating information in a way that readers are used to. The front page has space for a bio, which is alongside your contact information, socials, and affiliation. At the top right, you can list ongoing projects, your CV, contact information, and even a blog or photos or whatever else you'd like to include.

2. Horizontal: ([my website](https://www.trentwintermeier.com/)) I like this version, so this is what I'm using currently. I coded it myself, with the help of ChatGPT, so it's really basic but, I think, makes more sense to me as a beginner. In the repository, all we have is an index.html file and a folder for assets like images. On the website, I was inspired by [Virginia L. Montgomery](https://www.hellovlm.com/). The page scrolls, at large, horizontally, but each container scrolls vertically. I also like the overload of information this provides while also disrupting more traditional ways of engaging with a website.

Navigate to the GH repository page for the Jekyll-based site and click "Fork" up in the right side of the screen, next to "Watch" and "Star." This will create your own version of my repoistory as your own repository. Any changes either of us make to these repositories will not impact each other-- once you fork a repository, they become separated. All you are doing is copying this repository into your own account.

# Step 4: Publishing via GitHub Pages

With your own repository, you now have a complete copy of one of the websites. However, this isn't published online as of now. You just have the code sitting in your account, which is one of the reasons why people use GitHub: to store code. However, GH also allows users to create static sites with that code FOR FREE. To do this, follow these steps:

1. Click "Settings" on the top bar. It's at the end of the line that says "Code." Note that this is not your account settings but your repository settings, so everything you edit here will only apply to your repository that you're working in. 
2. Go to the bottom of the second section in the left side bar and click "Pages." This is where you'll access and configure the GitHub Pages function.
3. Under "Source" confirm that "Deploy from a branch" is selected. This is telling GitHub pages that we want to build a site from a branch (a section of code) in our repository. Below that, under "Branch," change the drop down from "None" to "Main." This identifies which branch (you only have 1) you want to publish as your site. A box should pop up to the right that says "/(root)"-- leave that as it is. Save if you need to.

It may take a minute to build-- which is to say that any time you make a change in GH to a repository using GitHub Pages, it will take a minute (depending on the type of change) to reflect that change. Since we just told GH to build an entire website, it can take a little longer, but it's still really quick. The status of these changes is reflected under the "Code" heading, next to your name and the name of the change. There should be a small orange dot (meaning in-progress), a green check (meaning done), or a red X (meaning failed). 

To see your site, which is just a copy of mine, go back to "Settings" and "Pages," and then at the top of that section there should be a box that reads "Your site s live at [link]." Click that link or "Visit Site" to see your published website. This is completely live, so anyone with this link can see this page. Notice that your website link is your GH username and repository name-- we'll talk about domains later.

# Step 5: Editing Your Website in GitHub

Editing your website requires familiarity with the repository that you've just forked. It also requires a little familiarity with Markdown or HTML ([here's a helpful style guide for beginners](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)). I'll identify some of the folders that we can work in and edit today, but you'll have to do the rest. To edit a page, click the pencil icon on the top right corner of a file. To save your change, click the green "Commit changes" button and confirm the commit. Refresh to see the status of your change.

<details closed>
<summary>1. Navigation pages: Under the "Data" folder, you can edit the titles for the navigation pages. Just go to "navigation.yml" and edit the name after "Title:." For example, you can change the title of "Publications" to "Research."</summary>
<br>
   - After we do this, we'll want to edit the page name and permalink to reflect the title change. Under the "Pages" folder (which holds the files of the navigation pages), find the "Publication.md" file and change the following:
   <br>
     - At the top, change the file name from "/_pages/publications.md" to "/_pages/research.md
      <br>
     - Title from "Publications" to "Research
      <br>
     - Permalink from "/publications/" to "/research/"
      <br>
     - You can also change the folder titled "_publications" to research.
</details>

<details closed>
<summary>2. Since we're under the "_publications" folder--or, now, what may be the "_research" folder-- let's look at adding research or publication information. The two files titled "publication1.md" and "publication2.md" is where you'll imput information on your research and/or publications. Upon clicking one of those files, you'll see where you can put that data in an section already styled for you. You just have to find and replace.
</summary>
<br>
   - Finding and replacing data under the other navigation titles is just as simple. Under the "_talks" folder, you'll see the file "_talk1.md" which is where you can put information on talks you've given.
   <br>
   - Under "_teaching" and, then, "class1.md," you can input information on the classes you've taught.
   <br>
     - However, if you have a second class you'd like to list, you will have to add a file.
   <br>
       - Click on "_teaching" and click "Add file" and "Create new file"
   <br>
       - Then, name it something like "class2.md" -- and you can always change these names to reflect your class names. Save this file.
   <br>
       - Go back to "class1.md" and copy the raw data. Paste this in the "class2.md" file and change the data to fit the new class you're adding. Save and you should see a second class under "Teaching" on your website.
</details>    

<details closed>
<summary>
3. Page name and author configuration: The "config.yml" file stores some of the important data for your site and also is where we can change the information for the page. Navigate to the "config.yml" and you can find where some of the language in your site corresponds to the code in this file. You can find and change the following:
   </summary>
   <br>
   - Under site settings, find the "title" column and change "My Homepage" to your name. This will change the title of the page in your browser tab and the name of the page on the site.
   <br>
   - Under site author, change "Name1 Name2" to your first and last name. You can change your bio, email, and add in other social links. The information following # shows you how to format code, which is helpful for the social links.
   </details>   

# Step 6: Editing Your Website with ChatGPT

ChatGPT can generate code that, in my experience, is very reliable if you know how to phrase your question right. This is a really helpful resource if you're new to coding and sometimes don't know either (1) what you're doing and/or (2) don't know how to look for what you want in your website. For example, say you want a 2 column CV under the CV header. What you need is two horizontal containers, which is difficult to know if you aren't familiar with HTML. If we ask Chatgpt to "In HTML, please write code for a 2-column CV for my website," it will give you code for two horizontal containers. ChatGPT bypasses the language needed to even begin to searching the internet, which is why I recommend using it for more complicated code. 

When I asked ChatGPT to develop this 2-column CV, below is the response, which can be copy and pasted in the CV.md file under "Pages". This comes up a little weird with the Jekyll style being used, so we may want to ask ChatGPT to generate a new format or to remove the box coming up at the top of the page. 

<details closed>
<summary>
   Response 1
</summary>
   
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your CV</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }

        .container {
            max-width: 960px;
            margin: 0 auto;
            padding: 20px;
            overflow: hidden;
        }

        header {
            background: #333;
            color: #ffffff;
            padding: 1em 0;
            text-align: center;
        }

        section {
            float: left;
            width: 70%;
        }

        aside {
            float: right;
            width: 30%;
            background: #ddd;
            padding: 20px;
        }

        h1, h2, h3 {
            color: #333;
        }

        ul {
            list-style-type: none;
            padding: 0;
        }

        ul li {
            margin-bottom: 10px;
        }
    </style>
</head>

<body>

    <header>
        <h1>Your Name</h1>
        <p>Web Developer</p>
    </header>

    <div class="container">

        <section>
            <h2>Summary</h2>
            <p>Your brief summary goes here.</p>

            <h2>Experience</h2>
            <h3>Job Title</h3>
            <p>Company Name, Location</p>
            <p>Date - Date</p>
            <ul>
                <li>Responsibility #1</li>
                <li>Responsibility #2</li>
            </ul>

            <!-- Add more experience sections as needed -->

            <h2>Education</h2>
            <h3>Degree</h3>
            <p>University Name, Location</p>
            <p>Date - Date</p>

            <!-- Add more education sections as needed -->

        </section>

        <aside>
            <h2>Contact</h2>
            <ul>
                <li>Email: your.email@example.com</li>
                <li>Phone: (123) 456-7890</li>
                <li>LinkedIn: linkedin.com/in/yourname</li>
                <li>GitHub: github.com/yourusername</li>
            </ul>

            <h2>Skills</h2>
            <ul>
                <li>HTML5</li>
                <li>CSS3</li>
                <li>JavaScript</li>
                <li>React</li>
                <!-- Add more skills as needed -->
            </ul>

            <!-- Add additional sections such as certifications, projects, etc. -->

        </aside>

    </div>

</body>

</html>
</details> 

Or, if you know what you want ChatGPT to generate, asking for the code can still be helpful as ChatGPT usually will write the entire document for you-- like the elements for the body, head, and etc. ChatGPT may also style what you're looking for, which you can delete, change, or keep. For example, I want to use an iframe for my CV that is in a Google Doc. If I ask ChatGPT to "Please write an iframe for my CV," this is the code I get: 

<details closed>
<summary>
   Response 2
</summary>
<!-- index.html -->
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Website</title>
</head>

<body>

    <h1>Welcome to My Website</h1>

    <iframe src="cv.html" width="800" height="1000" frameborder="0"></iframe>

    <!-- Additional content for your website -->

</body>

</html>
</details>

Now, all I need to do is put in the iframe for my CV. To do this, follow these steps:
1. Navigate to Google Docs and your CV document
2. Click "Edit" and then "Share"
3. Instead of "Link" click "Embed." Confirm your choice.
4. Copy the iframe

Once you have the iframe, just replace either the entire iframe line or the link in quotes. Now, when you update your CV, you don't have to update it in two places; just update the iframe link in your website. 

# Step 7: Connecting a Domain

While this website is free, the only part that you can choose to pay for is the domain. You don't have to do this; you can just direct people to the site's URL that GitHub generates for your (username + GitHub.io + repository name). It is quite long, though. I decided to use a domain because it was still cheaper than hosting a website on a site like SquareSpace, which is still $5 per month. I used Google Domains, which doesn't exist any more, but I'm guessing connecting domains to your site is pretty similar among providers. 

I decided to forward users instead of connecting the domain via GitHub. This way I can build different sites and switch between them more seamlessly. Basically, any time someone navigates to "www.trentwintermeier.com" or "trentwintermeier.com" they are forwarded to my GitHub URL. This is opposite to changing the domain in GitHub which actually changes the URL through GitHub pages. You can do the latter option in your settings and going to "Pages." If plan to change your site repository one day, or move from GitHub to Square Space (when you're making "big" academic money), you only need to update information with your domain provider.

For now, you can build as many websites as you'd like (for free!) and put the long URL somewhere or hyperlink it in other spaces. 
   
# You now have a free website! Woohoo!















