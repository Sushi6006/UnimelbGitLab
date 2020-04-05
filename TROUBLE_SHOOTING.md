# TROUBLE SHOOTING
These methods have solved problems me or my friends have encountered. Message me if you are not able to fix the same problem with the methods I have provided.

Before any trouble shooting, make sure you have completed the steps GitLab has instructed you to do.


## General Fix
You may use this method at **ANY** condition. These commands may fix everything you have problem with.

#### Method 1
Go to you study plan -> Withdraw from this subject.

#### Method 2
update your git config using the followings\
will do the job for the most of the time if you have encountered access problems when you have another git account on your computer
```
git config --global user.name "<your-username>"
git config --global user.email "<your-student-email"
git config --global credential.username "<your-username>"
git config --system --unset credential.helper
```
e.g. A student named "Bob C", with the username bobc
```
git config --global user.name "bobc"
git config --global user.email "bobc@student.unimelb.edu.au"
git config --global credential.username "bobc"
git config --system --unset credential.helper
```


## HTTP Basic: Access Denied
`HTTP Basic: Access Denied`
- click on your profile pic - top-right corner of the gitlab page
- settings
- "Access Tokens"
- add a new token with any name
- an expiry date you like (i used my graduation date)
- create
- ***REMEMBER TO COPY THE KEY SOMEWHERE SAFE AND YOU CAN FIND***
- connect to git (clone, add origin)
  - when entering the url, use \
    `https://<your-username>@gitlab...`
  - use the token key instead of the password
*Downside*: I have noticed that after using this method, everything needs to be done in `sudo`. 
