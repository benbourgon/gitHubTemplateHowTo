# How to create a template repo in GitHub
Instructions on how to create a template repo for sass file structure.

<em><strong>Note:</strong> These are just the methods I used. This is definitely not comprehensive - I am definitely open to changes or suggestions.</em>


<strong>Creating your template and pushing it to GitHub</strong>
1. Find an appropriate directory on your local computer to store your template folder.
2. Create your SASS file structure within that folder - as described <a href=https://github.com/HackerYou/bootcamp-notes/blob/main/stuff-you-need-to-know/resources-and-cheat-sheets/live-sass-setup.md>here</a>
3. Open up your browser and navigate to <a href=https://github.com>GitHub</a>.
4. Create a new repo to be your template, and call it whatever you want (i.e. sassTemplate).
5. Open your command line and cd into your template folder.
6. Enter "git init".
7. Stage and commit your files ("git add -A", then "git commit -m 'yourMessage'").
8. Enter "git remote add origin [and then your url here i.e.: https://github.com/yourusername/yourTemplateRepoName.git].
9. Enter "git branch -M main".
10. Enter "git push -u origin main".
11. Run a "remote -v" to check you've connected your repo to GitHub or refresh the repo on your browser to see the files you have pushed.
12. On your repo's page in your browser click Settings>General tab(should be the default tab) and then under Repository name, click "Template repository"<img width="1033" alt="Screen Shot 2022-03-12 at 12 13 30 PM" src="https://user-images.githubusercontent.com/22135594/158028257-0401375c-1f3c-486b-a3ec-7ec113963373.png">
13. You now have a template repo!
<hr>
<strong>Starting a new project using your template</strong>

These are the methods that I know of so far. There may be better/more efficient ways that don't know of.

<strong>Method 1</strong>: Clone

1. Open your command line and cd into the directory where you want your project's folder to live. Don't mkdir or create a folder there yet.
2. Enter "git clone [yourTemplatesURL.git]"
3. Rename the cloned folder as desired.
4. Open the cloned folder and delete the .git folder within.
5. cd into the folder in your command line and git init, add & commit.
6. Create a new repo in GitHub for your project
7. Enter "git remote add origin main [yourNewRepoURL.git]"
8. Enter "git branch -M main"
9. Enter "git push -u origin main"
10. Your new project is now ready to go!

<strong>Method 2</strong>: Pull

1. Open your command line and cd into the directory where you want your project's folder to be.
2. mkdir/create a project folder
3. cd into your project folder
4. Open your browser and navigate to [https://github.com/yourUsername/yourTemplateRepoName/generate/] to start a new repo from your template.
5. Name your repo and finish creating it. the files from the template will copy over as the first commit.
6. Enter "git init" into your command line.
7. Enter "git pull [yourNewProjectRepoURL.git]"
8. Enter "git remote add origin main [yourNewProjectRepoURL.git]"
9. Enter "git branch -M main"
10. (Optional) Make any changes to your files, stage and commit.
12. Enter "git push -u origin main"
13. Your new project is now ready to go!
