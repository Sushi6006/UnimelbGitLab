# How to Git
*From my experience, this is all you need to know for the simplest version control*
*I acknowledge that Visual Studio and many other editors have built-in git stuff, but I prefer using Terminal*

0. First of all, I recommend you to have a GitHub account

1. At the top right corner, you will see a plus logo: click and create a new repository
    - this will include all your project files.

2. Follow the instructions to complete creating your repository
    * name it whatever you want;
    * you can leave the description empty or you can write whatever you want;
    * I strongly recommend you make it private;
    * and I do not think you will need a README.md;
    * and leave the rest as default

3. You will be brought to a new page, and you will see\
   `https://github.com/[your username]/[the name of your repository].git` \
   \- copy this link.\
   **For private repo's** you need to change the url from the example above to:\
   `https://[your_username]:[your_password]:github.com/[your username]/[the name of your repository].git`\
   **OR**\
   `https://[your_username]:github.com/[your username]/[the name of your repository].git`\
   and enter your password when the terminal asks for it

   Otherwise, you will get a error saying
   ```
   remote: Repository not found.
   fatal: repository 'https://github.com/Sushi6006/unimelb_oosd_2019s2.git/' not found
   ```

4. Open up your terminal
    * `cd` to the directory you want to save your project/codes *no need to worry about creating a new empty directory, the next command will create a directory for you*
    * `git clone [your link here]` this will clone your repository to your device. If you did not create a README.md file, you will see a warning `warning: You appear to have cloned an empty repository.`, and that is totally fine.

Now, you have successfully created a repository and have a local copy of it on your device. You can upload everything you have to git as long as it is in your directory (cloned from git).
* to upload(push) files (update to GitHub)
  * `cd` to your directory. It will be something like .../[the name of your repository]
  * `git add -A` - this will add all files to git
  * `git commit` or `git commit -m [message]` to commit everything to git, `-m` to include a commit message **this will not be uploaded to GitHub**
  * `git push` to push all your files to git
  and now, you will be able to see all your files on your GitHub repository in your browser
* to update your local files
  * `cd` to your directory.
  * `git pull` to download what you have on GitHub
  You will only use this if you make changes on GitHub or through elsewhere (which is basically never)
