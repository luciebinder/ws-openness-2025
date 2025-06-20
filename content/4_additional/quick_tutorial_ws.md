# Quick Setup Guide 

Okay, now let's get started! With your own course concept in mind, you will learn now how to create and host your Jupyter Book course website. 


If you have any questions, feel free to click on the section titels to dive into the detailed tutorials or get in touch with me! 

## 1. [Set up your GitHub account](../1_github/account)
If you haven't already set up your GitHub account, please go to the [respective section](../1_github/account).  

## 2. [Copy our course template](../1_github/project)
Let's copy our ready-to-go course template! It’s the quickest way to get started — simply customize and add your own pages to fit your content, without worrying about setting up a project from scratch. 

1\. Go to the GitHub page of our [course template](https://github.com/luciebinder/course-template-minimal) and click on "fork".

![depicting position a look of the fork button on a GitHub repository](../../static/fork-button.png)

2\. Give your course a name and a description, check the box "Copy the main branch only," and click the "Create fork" button.

![depicting position a look of the fork button on a GitHub repository](../../static/create-fork.png)

## 3. [Getting familiar with the course template](../1_github/template)
Let's take a look into the structure of the course template:

![depicting the contents of the course template repository on GitHub](../../static/folder-structure_minimal-template.png)

Some files can be ignored, as they contain technical information for hosting the website. The majority of what you'll be modifying is located in the "lecture" content folder, which looks like this:

![depicting the contents of the course template repository on GitHub](../../static/lecture-folder-structure.png)

In this folder, you can add your content by editing or adding Markdown files.

## 4. [Edit a file](https://luciebinder.github.io/ws-openness-2025/content/1_github/template.html#make-your-first-adjustments)

Let's edit your first file, the `_config.yml` file! Here, you'll update the course title, authors' names, affiliations, and other key details to make the template your own.

1\. To edit a file, click on the specific file (here: `_config.yml`). 

![Image of the file structure.](../../static/click_on_file.png)

2\. Click the edit button, represented by a small pencil in the upper right corner. 

![Image of the edit button on the upper right corner.](../../static/edit_file.png)

3\. Replace the existing information with your course title, your name, affiliation, and any other relevant details. Once you're finished, click "Commit changes...".

![Image of the commit changes button.](../../static/commit_changes.png)

4\. For transparency and version control, provide a brief message describing the changes you made.

![Image of the pop-up window in which one can write the commit message](../../static/commit_message.png)

As soon as you click on "Commit changes", your changes will be saved.

**Awesome! You’ve just added your first personal touch!**

The next step is to adjust a few settings so that GitHub Pages can host your website and automatically update it whenever you make changes.

## 5. [Host your course website](../2_host/host_website)

1\. At the top of your repository, click on “Settings”.

![Image of the tab where the word "Settings" is located on the far right](../../static/settings.png)

2\. On the left side, click on "Pages".

![Image of the menu on the left side.](../../static/pages.png)
  
3\. Under Source, make sure that "Deploy from a branch" is selected.

![Image of the deploy from branch setting.](../../static/deploy-from-branch.png) 

4\. Under Branch: Select branch “main”. The folder “/root” is automatically selected.

![Image of the settings under Branch.](../../static/branch.png)

This should look like this now. Don't forget to click on save.

![Image of the settings under Branch.](../../static/save-branch.png)

5\. Click on "Action" and then "General" on the left side.

![Image of the menu on the left side.](../../static/actions-general.png)

6\. At the bottom of the page, under "Workflow permissions," select the option "Read and write permissions" and allow Github Actions to create and approve pull requests. Then, click on save.

![Image of the workflow permissions.](../../static/workflow_permissions.png)

7\. Now we need to push a new commit to your repo, i.e. make a change to one file in order to start the workflow process in the background.

Let's do this together by adding some text to the `README` file, a file that entails some main information on your course. 

Click on "Code" to get back to your file structure. Then, click on the `README` file. 

![Image of the upper options, selecting Code.](../../static/code.png)

Click on the "edit" symbol: 

![Image of the edit button.](../../static/edit-readme.png)

Enter some text and click on "commit changes" when you're done.

![Image of the README file that is edited.](../../static/edit-readme2.png)

Commit the changes and add some descriptions about your changes:

![Image of the commit process.](../../static/commit-readme.png)

Great! Now you changed one file and GitHub Pages starts running a workflow in the background. Let's check the worflows!

8\. Click on "Actions" at the top of your repository. You should see a workflow called "pages build and deployment" running (indicated by the yellow circle). Don't worry that the first process(es) failed (indicated by the red symbol)! That’s expected, since we had to adjust the workflow settings first.

![Image of the workflow "pages build and deployment" with a green checkmark.](../../static/action-click.png)

Wait until the process is complete, indicated by a green checkmark:

![Image of the workflow "pages build and deployment" with a green checkmark.](../../static/green-checkmark.png)

9\. Go back to "Settings", and then "Pages". Select "gh-pages" (instead of "main") as branch.
    
![Image of the settings under Branch.](../../static/gh-pages.png)

10\. Finally, on the top of this page, under "GitHub Pages", you should now find a field that looks like this:

![Image of the final link that is presented under "GitHub Pages".](../../static/pages_link.png)

This is the link to your newly built website! When you click the link, you might notice that there's no table of contents yet and only the README file is displayed. Don’t worry — we just need to make one more commit!

11\. Push a last commit to your repository. You might want to copy your link and paste it into your `README` file.

![Image of the README file with the link added.](../../static/edit-readme3.png)

As soon as you committed your changes and the workflow under "Actions" shows a green checkmark, you can refresh your website! 

Congratulations! You should see the welcome page to your website. Now it's your turn to fill the pages.


# What are the next steps?

## 6. [Create content](../3_create/intro)

Open an existing Markdown (.md) or Jupyter notebook (.ipynb) file or create a new one and copy your interactive content and code. Make sure to give each file a meaningful name and add a title to each page.

## 7. [Update Table of Contents](../3_create/setup-files)

Once you've created files, open the `_toc.yml`. Add your newly created files in the sequence of your choice according to our template.

## 8. [Update the README file](https://luciebinder.github.io/ws-openness-2025/content/1_github/template.html#the-readme)

Open the `README.md` file and update the information on your course.
