# Creating-repository-in-github-using-ssh-Git

Steps-

```

1. Generating a new SSH key
$ ssh-keygen -t rsa -b 4096 -C "<your_email@example.com>"

2. Add the SSH key to the GitHub account
$ cat < ~/.ssh/id_rsa.pub
- Go to github.com and click on the profile photo in the upper-right corner
- Click on the Settings button and navigate to SSH and GPG Keys
- Click on the New SSH Key button
- Enter the Title as mySSHKey and Key (copy paste the key that is displayed in your terminal) and click on the Add SSH key button

3. Creating a repository on the local machine
- mkdir creating-repository-in-github-using-ssh
- cd creating-repository-in-github-using-ssh
- echo "# creating-repository-in-github-using-ssh" >> README.md
- git init
- git add README.md
- git commit -m "first commit"
- git branch -M main

4. Create a GitHub repository
- Go to github.com and log in to your account
- Click on the New button to create a new repository named as creating-repository-in-github-using-ssh

5. Add a remote repository using the SSH URL
$ git remote add origin SSH_URL 
- Execute git remote -v command to check the remote repository

6. Push the changes in the local repository to GitHub
$ git push -u origin main
$ git status
Go to github.com and check the remote repository

```

